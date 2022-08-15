<script>
    import {Link} from "svelte-routing";
  </script>
  
  <button class="backButton"> <Link to="/" style="color: white;"> <span>Torna a l'inici</span> </Link> </button>
  
  <style>
      .backButton {
        display: inline-block;
        vertical-align:middle;
        background-color: #65C66E;
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
      
      .backButton span {
        cursor: pointer;
        display: inline-block;
        position: relative;
        transition: 0.5s;
      }
      
      .backButton span:after {
        content: '\00bb';
        position: absolute; 
        opacity: 0;
        top: 0;
        right: -20px;
        transition: 0.5s;
      }
      
      .backButton:hover span {
        padding-right: 25px;
      }
      
      .backButton:hover span:after {
        opacity: 1;
        right: 0;
      }
      </style>