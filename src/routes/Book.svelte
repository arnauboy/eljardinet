<script>
  import Header from "../components/Header.svelte";
  import Icons from "../components/Icons.svelte";
  import {Link} from "svelte-routing";
  </script>
  
  <svelte:head>
    <title>Reserva</title>
  </svelte:head>
  
  <Header route="book" />
  <Icons />
  <div style = "max-width: 70%; text-align: left; margin: 100px auto;">
    <h1>Reserva</h1>

    Servei no disponible temporalment. Per reserar contacta amb nosaltres a través de la pàgina de <Link to="/contact" style="text-decoration: none;" > contacte </Link>.
   
  </div>
  