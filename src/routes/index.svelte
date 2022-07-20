<script>
  import Search from "../lib/Search.svelte";
  import Projects from "../lib/FeaturedProjects.svelte";
  import ContactForm from "../lib/ContactForm.svelte";
  import Developers from "../lib/FeaturedDevelopers.svelte";

</script>

<main class="main">
  <div class="hero-img"></div>
  <h1 class="title">find your <br> space now</h1>
  <Search/>
</main>
<Projects/>
<Developers/>
<ContactForm/>





<style>
  .main{
    width: 100vw;
    min-height: 100vh;
    padding-top: calc( var(--header-height) + 120px) ;
  }
  .hero-img{
    width: 100%;
    /* min-height: 100vh; */
    height: 100%;
    background: url('../hero-img.png');
    background-repeat: no-repeat;
    /* background-position: top left; */
    background-position: center;
    background-size: cover;
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
  .title{
    font-size: 80px;
    font-weight: bold;
    color: white;
    text-align: center;
    text-transform: capitalize;
  }
  
</style>