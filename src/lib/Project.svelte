<script>
  export let project;
</script>

<a href={project.link} class="project">

    <div class="details">
      <h2 class="name">{project.name}</h2>
      <p class="price">starting price<span>{project.startingPrice} EGP</span></p>
    </div>

</a>

<style>
  .project{
    background: url("../p1.png") center no-repeat;
    background-size: cover;
    display: block;
    min-height: 400px;
    position: relative;
    margin-bottom: 24px;
    overflow: hidden;
  }
  .project:nth-child(4){
    height: 600px;
  }
  .project:hover{
    transform: scale(1.1);
    transition:transform  .4s;
  }
  .details{
    color: white;
    padding: 16px 24px;
    background-color: rgba(0,0,0,.3);
    width:100% ;
    text-transform: capitalize;
    position: absolute;
    bottom: 0;
  }
  .name{
    font-weight: bold;
  }
  .price{
    margin-top: 16px;
    color: #c5c5c5;
  }
  .price span{
    color: white;
    /* display: block; */
    /* margin-top: 8px; */
    margin-left: 8px;
    font-weight: bold;
  }
  
</style>