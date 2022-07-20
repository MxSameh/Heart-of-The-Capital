<script>
  
</script>

<header class="header">
  <!-- LOGO -->
  <a href="/">
    <img class="logo-img" src="../logo-white.png" alt="heart of the capital logo">
  </a>

  <!-- PAGES NAVIGATION -->
  <nav class="nav">
      <a href="/" class="nav-item">home</a>
      <li class="nav-item">projects</li>
      <li class="nav-item">developers</li>
      <a href="/about-us" class="nav-item">about</a>
      <a href="/contact" class="nav-item">contact</a>
  </nav>

  <!-- ICONS NAVIGATION -->
  <nav class="nav">

    <!-- phone Logo -->
    <svg class="nav-icon phone-logo" viewBox="0 0 60 60" xmlns="http://www.w3.org/2000/svg">
      <path d="M52.7402 55.9999C25.0145 56.0389 3.97078 34.745 4.00003 7.25975C4.00003 5.4625 5.45603 4 7.25003 4H15.83C17.4388 4 18.807 5.183 19.0443 6.7755C19.6101 10.5944 20.721 14.3124 22.343 17.8157L22.6778 18.5372C22.9026 19.0228 22.951 19.5715 22.8145 20.0889C22.6781 20.6063 22.3653 21.0598 21.9303 21.3712C19.2718 23.2692 18.2578 27.088 20.328 30.065C22.9345 33.8133 26.1876 37.0675 29.935 39.6752C32.9152 41.7422 36.734 40.7282 38.6287 38.073C38.9399 37.6366 39.3938 37.3227 39.9119 37.1856C40.43 37.0485 40.9797 37.0968 41.466 37.3222L42.1842 37.6537C45.6877 39.2787 49.4057 40.3902 53.2245 40.9557C54.817 41.193 56 42.5612 56 44.1732V52.7499C56 53.177 55.9158 53.5999 55.7523 53.9944C55.5887 54.3889 55.3491 54.7474 55.0469 55.0492C54.7448 55.351 54.3861 55.5904 53.9914 55.7535C53.5968 55.9166 53.1738 56.0004 52.7467 55.9999H52.7402Z" />
    </svg>

    <!-- Pin Logo -->
    <svg class="nav-icon pin-logo" viewBox="0 0 60 60" xmlns="http://www.w3.org/2000/svg">
      <path d="M30 3.75C24.5319 3.75645 19.2896 5.93151 15.4231 9.79805C11.5565 13.6646 9.38147 18.9069 9.37502 24.375C9.36847 28.8435 10.8281 33.1908 13.53 36.75C13.53 36.75 14.0925 37.4906 14.1844 37.5975L30 56.25L45.8231 37.5881C45.9056 37.4888 46.47 36.75 46.47 36.75L46.4719 36.7444C49.1725 33.1868 50.6314 28.8415 50.625 24.375C50.6186 18.9069 48.4435 13.6646 44.577 9.79805C40.7104 5.93151 35.4681 3.75645 30 3.75V3.75ZM30 31.875C28.5167 31.875 27.0666 31.4351 25.8332 30.611C24.5999 29.7869 23.6386 28.6156 23.0709 27.2451C22.5033 25.8747 22.3547 24.3667 22.6441 22.9118C22.9335 21.457 23.6478 20.1206 24.6967 19.0717C25.7456 18.0228 27.082 17.3085 28.5368 17.0191C29.9917 16.7297 31.4997 16.8782 32.8701 17.4459C34.2406 18.0136 35.4119 18.9749 36.236 20.2082C37.0602 21.4416 37.5 22.8916 37.5 24.375C37.4975 26.3634 36.7066 28.2696 35.3006 29.6756C33.8946 31.0815 31.9884 31.8725 30 31.875V31.875Z"/>
    </svg>

  </nav>

</header>

<style>
  .header{
    align-items: center;
    color: white;
    display: flex;
    justify-content: space-between;
    padding: 24px 40px;
    position: absolute;
    width: 100%;
  }
  .logo-img{
    width: 200px;
  }
  .logo-img:hover{
    cursor:pointer ;
  }
  .nav{
    display: flex;
  }
  .nav-item{
    font-size: 24px;
    font-weight: 500;
    text-transform: capitalize;
    color: white;
  }
  .nav-item:hover{
    cursor: pointer;
    text-decoration: underline;
  }
  .nav-item:not(:last-child){
    margin-right: 24px;
  }
  .nav-icon{
    width: 30px;
    fill: white;
  }
  .nav-icon:hover{
    cursor: pointer;
    fill: #e0e0e0;
  }
  .phone-logo{
    margin-right: 16px;
  }
</style>