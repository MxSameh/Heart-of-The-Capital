<script>
  import '../styles/main.css'
  import Header from "../lib/Header.svelte";
  import Footer from "../lib/Footer.svelte";
</script>

<Header/>
<div class="wrapper">
  <slot />
</div>
<Footer/>



<style>

  .wrapper{
    min-height: calc( 100vh - var(--footer-height))
  }
  
</style>