<script>
</script>
  
  <button class="bookButton" style="vertical-align:middle"> <a href="https://www.booking.com/hotel/es/el-jardinet.ca.html" style ="color: white"> <span>Booking.com</span> </a> </button>
  
  <style>
      .bookButton {
        display: inline-block;
        border-radius: 50px; 
        background-color: #003580;
        border: none;
        color: #FFFFFF;
        text-align: center;
        font-size: 18px;
        padding: 15px;
        width: 150px;
        transition: all 0.5s;
        cursor: pointer;
        margin: 5px;
        text-decoration: none;
      }
      
      .bookButton span {
        cursor: pointer;
        display: inline-block;
        position: relative;
        transition: 0.5s;
      }
      
      .bookButton span:after {
        content: '\00bb';
        position: absolute; 
        opacity: 0;
        top: 0;
        right: -20px;
        transition: 0.5s;
      }
      
      .bookButton:hover span {
        padding-right: 25px;
      }
      
      .bookButton:hover span:after {
        opacity: 1;
        right: 0;
      }
      </style>