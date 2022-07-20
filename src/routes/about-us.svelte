<script>
  let members = [
    {id:1 , name:'Mr. Ahmed Fathy',title:'CEO / Founder'},
    {id:2 , name:'Mrs. Sarah Mohamed ',title:'Manging Partner'},
    {id:3 , name:'Mr. Mahmoud Fathy',title:'Manging Partner'},
    {id:4 , name:'Mr. Ahmed Hesham',title:'Team Leader'},
  ]
  
</script>

<div class="header"></div>
<section class="who">

  <h1 class="title">who are we</h1>
  <div class="text-container">
    <p class="text">HOTC is a leading company in consulting people on where and why to put their money in a specific area. Our team is customer's oriented, highly-professional, and knowledgeable. They are highly trained to lead a great experience for our clients through all means of professionalism, integrity, and honesty.
    HOTC gives specialized financial, investment, and ownership advice to all who are looking to buy a new property from first home, second home, commercial, administrative, and medical.
    </p>
    <p class="text">Our social responsibility is to make sure that our clients are investing in the right place and to end up their investment in the time they consider within a winning situation.  
    HOTC was not founded to sell anything but to direct potential buyers toward the best fit that matches their needs and priorities. 
    </p>
  </div>

</section>

<section class="board">
  <h1 class="title">Board of Directors</h1>
  <ul class="board-list">
      {#each members as member (member.id) }
      <li class="member">
        <div class="img"></div>  
        <h2 class="name"> {member.name} </h2>
        <span class="position"> {member.title} </span>
      </li>
      {/each}

  </ul>

</section>

<section class="where">
  <h1 class="title">where to find us</h1>
</section>

<style>
  .header{
    width:100% ;
    height: var(--header-height);
    background-color: black;
  }
  .who{
    padding: 0 40px;
    margin-top: 120px;
  }
  .title{
    border-left: 4px solid #c0c0c0;
    font-size: 40px;
    padding: 0 16px;
    text-transform: capitalize;
    text-align: left;
  }
  .text-container{
    display: flex;
    margin-top: 40px;
    gap: 24px;
  }
  .text{
    flex-basis: 100%;
    font-size:24px;
    line-height: 36px;
    color: #333;
  }
  .board{
    padding: 0 40px;
    margin-top: 80px;
  }
  .board-list{
    margin: 40px auto 0 ;
    display: flex;
    width:fit-content ;
    max-width: 100%;
    flex-wrap: wrap;
    row-gap: 32px;
    column-gap: 80px;
  }
  /* .member:not(:last-child){
    margin-right: 80px;
  } */
  .img{
    width: 200px;
    height: 200px;
    border-radius: 100%;
    background-color: rgb(158, 156, 156);
  }
  .name{
    text-transform: capitalize;
    font-size: 24px;
    text-align: center;
    margin-top: 32px;
  }
  .position{
    font-size: 24px;
    margin-top:16px;
    text-align: center;
    display: block;
    color:#333 ;
  }
  .where{
    padding: 0 40px;
    margin-top: 80px;
  }
  
</style>