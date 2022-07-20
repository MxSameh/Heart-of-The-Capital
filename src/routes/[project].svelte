<script>
  import ProjectDetails from "../lib/ProjectDetails.svelte";
  import ProjectLocation from "../lib/ProjectLocation.svelte";
  import ProjectUnits from "../lib/ProjectUnits.svelte";
  
</script>

<main>
<div class="hero-img"></div>
<h1 class="project-name">creek town</h1>
</main>
<ProjectDetails />
<ProjectUnits />
<ProjectLocation/>


<style>
  main{
    width: 100vw;
    height: 100vh;
    display: flex;
  }

  .hero-img{
    width: 100vw;
    min-height: 100vh;
    background: url('../hero-img.png') center center no-repeat ;
    position: absolute;
    top:0;
    z-index: -1;
  }
  .hero-img::before{
    content:'';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    background:rgba(0,0,0,.3) ;
  }
  .project-name{
    font-size: 64px;
    color: white;
    text-transform: capitalize;
    margin:auto 0 40px 40px;
  }
  
</style>