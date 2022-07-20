<script>
  export let unit;
</script>

<div class="unit">
  <div class="image"></div>

  <div class="unit-info">

    <div class="bedrooms info">
      <svg class="bed-icon" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
        <path d="M3.42857 3C2.01857 3 0.857143 4.16143 0.857143 5.57143V11.3829C0.334286 11.856 0 12.5331 0 13.2857V21H4.28571V19.2857H19.7143V21H24V13.2857C24 12.5331 23.6657 11.856 23.1429 11.3829V5.57143C23.1429 4.16143 21.9814 3 20.5714 3H3.42857ZM3.42857 4.71429H20.5714C21.0471 4.71429 21.4286 5.09571 21.4286 5.57143V10.7143H19.7143V9.85714C19.7143 8.44714 18.5529 7.28571 17.1429 7.28571H13.7143C13.0569 7.28571 12.4569 7.54286 12 7.95429C11.5313 7.52655 10.9203 7.28827 10.2857 7.28571H6.85714C5.44714 7.28571 4.28571 8.44714 4.28571 9.85714V10.7143H2.57143V5.57143C2.57143 5.09571 2.95286 4.71429 3.42857 4.71429ZM6.85714 9H10.2857C10.7614 9 11.1429 9.38143 11.1429 9.85714V10.7143H6V9.85714C6 9.38143 6.38143 9 6.85714 9ZM13.7143 9H17.1429C17.6186 9 18 9.38143 18 9.85714V10.7143H12.8571V9.85714C12.8571 9.38143 13.2386 9 13.7143 9ZM2.57143 12.4286H21.4286C21.9043 12.4286 22.2857 12.81 22.2857 13.2857V19.2857H21.4286V17.5714H2.57143V19.2857H1.71429V13.2857C1.71429 12.81 2.09571 12.4286 2.57143 12.4286Z" />
      </svg>
      <span>{unit.bedrooms} Bedrooms</span>
    </div>

    <div class="area info">
      <svg class="area-icon" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
        <path d="M3 19C3 19.5304 3.21071 20.0391 3.58579 20.4142C3.96086 20.7893 4.46957 21 5 21H19C19.5304 21 20.0391 20.7893 20.4142 20.4142C20.7893 20.0391 21 19.5304 21 19V5C21 4.46957 20.7893 3.96086 20.4142 3.58579C20.0391 3.21071 19.5304 3 19 3H5C4.46957 3 3.96086 3.21071 3.58579 3.58579C3.21071 3.96086 3 4.46957 3 5V19ZM12 6H18V12H16V8H12V6ZM6 12H8V16H12V18H6V12Z" />
      </svg>
      <span>{unit.minArea} - {unit.maxArea} sqm</span>
    </div>

    <div class="bathrooms info">
      <svg class="bath-icon" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
        <path d="M1.5 18C1.5 19.3275 2.08547 20.5087 3 21.3323V23.25C3 23.6625 3.33562 24 3.75 24H5.25C5.6625 24 6 23.6625 6 23.25V22.5422H18V23.25C18 23.6642 18.3358 24 18.75 24H20.25C20.6642 24 21 23.6642 21 23.25V21.3328C21.9145 20.5092 22.5 19.328 22.5 18.0005V16.5H1.5V18ZM23.25 12H4.5V3.62109C4.49859 3.11484 5.20312 2.82328 5.55937 3.18187L6.20625 3.82781C5.79375 5.09063 6.06562 6.30469 6.75937 7.18125C6.46406 7.47656 6.45938 7.95938 6.75 8.25L7.28016 8.78016C7.57303 9.07303 8.04797 9.07303 8.34094 8.78016L13.2816 3.83953C13.5744 3.54666 13.5744 3.07172 13.2816 2.77875L12.7514 2.24859C12.4585 1.95572 11.9836 1.95572 11.6906 2.24859C10.8141 1.55906 9.59531 1.29141 8.32969 1.70672L7.68281 1.06125C7.00781 0.386719 6.075 0 5.12344 0C3.12469 0 1.5 1.62469 1.5 3.62109V12.0023L0.75 12C0.335812 12 0 12.3375 0 12.75V14.25C0 14.6625 0.335812 15 0.75 15H23.25C23.6642 15 24 14.6642 24 14.25V12.75C24 12.3375 23.6625 12 23.25 12Z" />
      </svg>
      <span>{unit.bathrooms} Bathrooms</span>
    </div>

  </div>

  <div class="unit-details">
    <div class="price">
      <p>starting price <span>{unit.startingPrice} egp</span></p>
    </div>

    <button class="view-btn">view</button>
  </div>



</div>

<style>
  .unit{
    background-color: white;
    border-radius: 32px;
  }
  .unit:not(:last-child){
    margin-right: 40px;
  }

  .image{
    width: 450px;
    height: 400px;
    background-color: black;
    border-radius: 32px;
  }
  .unit-info{
    padding: 0 40px;
    margin-top: 40px;
    display: grid; 
    grid-template-columns: 1fr 1fr;
    row-gap: 16px;
  }
  .info{
    display: flex;
    align-items: center;
    width:fit-content ;
  }
  .area{
    justify-self: end;
  }
  svg{
    width:24px ;
    fill: black;
  }
.info span{
  font-size: 24px;
  margin-left: 12px;
}

.unit-details{
  margin: 32px 0 40px;
  display: flex;
  justify-content: space-between;
  align-items: flex-end;
  padding: 0 40px;
}

.price p{
  font-size: 24px;
  text-transform: capitalize;
  color: #333;
}

.price span{
  font-weight: bold;
  text-transform: uppercase;
  display: block;
  color: black;
  letter-spacing: 1px;
  margin-top: 8px;
  margin-left: 4px;
}

.view-btn{
  padding: 12px 28px;
  font-size: 24px;
  line-height: 24px;
  background-color: black;
  color: white;
  border-radius: 8px;
  text-transform: capitalize;
}




  
</style>