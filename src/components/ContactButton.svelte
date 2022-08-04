<script>
  import { Router, Link, Route } from "svelte-routing";
</script>

<button class="bookButton" style="vertical-align:middle"> <Link to="contact" style="color: #65C66E"> <span> Contacte </span> </Link> </button>

<style>
    .bookButton {
      display: inline-block;
      border-radius: 50px;
      background-color: white;
      border: 1px solid;
      border-color: #65C66E;
      color: #65C66E;;
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