<script>
  import Header from "../components/Header.svelte";
  import Icons from "../components/Icons.svelte";
  </script>
  
  <svelte:head>
    <title>Reserva</title>
  </svelte:head>
  
  <Header route="book" />
  <Icons />
  <div style = "max-width: 70%; text-align: left; margin: 100px auto;">
    <h1>Reserva</h1>

    Calendari on escullir dates

    Afegir reserva - mostrar preu - pop up demanar correu electrònic i telèfon mòbil
   
  </div>
  
  <style>
    p {
      font-size: 1.2em;
    }
  </style>