<script>
	import BookButton from './../components/BookButton.svelte';
    import Header from '../components/Header.svelte';
    import Icons from '../components/Icons.svelte';
	import ReservaHeader from '../components/ReservaHeader.svelte';
	import Album from '../components/Album.svelte';
	import Description from '../components/Description.svelte';
	import Installacions from '../components/Installacions.svelte';
</script>

<svelte:head>
	<title>El Jardinet</title>
</svelte:head>


<Header route="/"/>
<Icons />
<ReservaHeader />
<div style = "max-width: 70%; text-align: left; margin: 0 auto;">
	<Description />
	<hr />	
	<Installacions />
	<hr />
	<Album />
	<p style = "font-size: 1.2em"> Seguiu-nos a instagram a <a href="https://instagram.com/eljardinetdeborreda" alt="">@eljardinetdeborreda</a> per a veure més fotografies i no perdreus cap novetat!</p>
</div>


<style>
</style>