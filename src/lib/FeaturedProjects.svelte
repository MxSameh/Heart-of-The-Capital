<script>
  import Project from "./Project.svelte";
  let projects = [
    {id:1, name:'mivida', img:'./p1.png', link:'/projects/mivida', startingPrice:'1,200,000'},
    {id:2, name:'creek town', img:'./p2.png', link:'/projects/creek-town', startingPrice:'1,400,000'},
    {id:3, name:'hyde park', img:'./p1.png', link:'/projects/hydepark', startingPrice:'2,000,000'},
    {id:4, name:'heceinda', img:'./p2.png', link:'/projects/heceinda', startingPrice:'2,000,400'},
    {id:5, name:'marasi', img:'./p1.png', link:'/projects/marasi', startingPrice:'1,700,00'},
    {id:6, name:'zed', img:'./p1.png', link:'/projects/zed', startingPrice:'1,700,00'},
    {id:7, name:'badya', img:'./p1.png', link:'/projects/badya', startingPrice:'1,700,00'},
  ]

</script>

<section class="featured-projects">
  
  <div class="section-header">
    <h2 class="title">top projects this month</h2>
    <a href="/">explore all</a>
  </div>

  <div class="projects-list">
    {#each projects as project (project.id) }
      <Project {project}/>
      {/each}
  </div>
</section>

<style>
  .featured-projects{
    padding: 0 var(--page-padding);
    margin-top: 80px;
  }
  .section-header{
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .title{
    font-size: 40px;
    font-weight: bold;
    color: #333;
    text-transform: capitalize;
  }
  .section-header a {
    color: black;
    font-size: 24px;
    text-transform: capitalize;
  }
  .projects-list{
    margin-top: 40px;
    column-count: 3;
    -moz-column-count: 3;
    -webkit-column-count: 3;
    column-width: 33%;
    -moz-column-width: 33%;
    -webkit-column-width: 33%;
    column-gap: 24px;
  }
</style>