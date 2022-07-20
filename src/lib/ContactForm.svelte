<script>
  
</script>

<section>
  <h1 class="title">let us help you find your perfect place</h1>
  <p class="sub-title">Proffesional property consultans are always available to answer your questions and help you finding what you looking for.</p>
  <form on:submit|preventDefault>
    <input id="name" type="text" placeholder="Enter Your Name">

    <div class="number-wrapper">
      <input id="number" type="text" placeholder="Enter Your Number">
      <button >get help</button>
    </div>

  </form>
</section>

<style>
  section{
    margin-top: 120px;
    padding:80px 40px;
    background-color: #F2F2F2;
  }
  .title{
    font-size: 40px;
    text-transform: uppercase;
    text-align: center;
  }
  .sub-title{
    margin-top: 16px;
    color:#555;
    text-align: center;
    font-size: 24px;
  }
  form{
    margin: 40px auto 0;
    width: 70vw;
    max-width: 700px;
  }
  input{
    padding: 13px 16px;
    border-radius:4px ;
    font-size: 16px;
  }
  #name{
    width:100%;
    margin-bottom: 24px;
  }
  #number{
    width: 80%;
  }
  .number-wrapper{
    display: flex;
    align-items: flex-start;
    gap: 5%;
  }

  button{
    background-color: black;
    border-radius:4px ;
    color: white;
    font-size: 20px;
    font-weight: bold;
    height: 42px;
    text-transform: capitalize;
    padding: auto 16px;
    width:15%;
  }
  button:hover{
    cursor: pointer;
    background-color: #222;
  }

</style>