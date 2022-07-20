<script>
  import Unit from "./unit.svelte";

  let units = [
     {id:1, img:'./p2.png', bedrooms:1, bathrooms:1, minArea: 60, maxArea: 80, startingPrice:'1,200,000'},
     {id:2, img:'./p1.png', bedrooms:2, bathrooms:2, minArea: 120, maxArea: 160, startingPrice:'1,700,000'},
     {id:3, img:'./p2.png', bedrooms:3, bathrooms:2, minArea: 180, maxArea: 221, startingPrice:'2,400,000'},
     {id:4, img:'./p1.png', bedrooms:3, bathrooms:3, minArea: 200, maxArea: 270, startingPrice:'3,000,000'},
  ]
  
</script>

<section>
  <h1 class="title">properties</h1>
  <div class="wrapper">

    <nav class="nav">
      <span class="nav-item active-tab">apartments</span>
      <span class="nav-item">villas</span>
      <span class="nav-item">others</span>
    </nav>

    <div class="units-list">
      {#each units as unit (unit.id) }
        <Unit {unit}/> 
      {/each}
    </div>

  </div>
</section>

<style>
  section{
    margin-top: 80px;
  }
  .title{
    border-left: 4px solid #c0c0c0;
    font-size: 40px;
    margin-left: 40px;
    padding: 0 16px;
    text-transform: capitalize;
    text-align: left;
  }
  .wrapper{
    margin-top: 40px;
    background-color: #e1e1e1;
    padding: 40px;
  }
  .nav{
    width:100% ;
  }
  .nav-item{
    text-transform: capitalize;
    font-size: 24px;
    font-weight: 500;
  }
  .nav-item:not(:last-child){
    margin-right: 40px;
  }
  .nav-item:hover{
    cursor: pointer;
  }
  .active-tab{
    padding-bottom:8px ;
    border-bottom: 2px solid var(--yellow);

  }
  .units-list{
    display: flex;
    margin-top: 48px;
    overflow-x: hidden;
  }
  
</style>