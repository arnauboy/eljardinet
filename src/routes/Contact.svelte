<script>
import Header from "../components/Header.svelte";
import Icons from "../components/Icons.svelte";
</script>

<svelte:head>
  <title>Contacte</title>
</svelte:head>

<Header route="contact" />
<Icons />
<div style = "max-width: 70%; text-align: left; margin: 100px auto;">
  <h1>Contacte el Jardinet de Borredà</h1>
  <p>Posa't en contacte amb nosaltres si vols fer una reserva, ja sigui través del telèfon móbil o el correu electrònic.
  No dubtis en consultar-nos qualsevol dubte!

  <p>Telèfon: +34 679701399</p>
  <p>Correu electrònic: joan_miquel@msn.com</p>
  <p>Missatge directe a Instagram: <a href="https://instagram.com/eljardinetdeborreda">@eljardinetdeborreda</a> </p>
</div>

<style>
  p {
    font-size: 1.2em;
  }
</style>