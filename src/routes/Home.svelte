<script>
	import BookButton from './../components/BookButton.svelte';
    import Header from '../components/Header.svelte';
    import Icons from '../components/Icons.svelte';
	import ReservaHeader from '../components/ReservaHeader.svelte';
import Album from '../components/Album.svelte';
</script>

<svelte:head>
	<title>El Jardinet</title>
</svelte:head>

<main>
	<Header />
    <Icons />
	<ReservaHeader />
	<div style = "max-width: 70%; text-align: left; margin: 0 auto;">
		<p class = "features"> <img src = "images/jardi.png" alt = "jardi" class = "little-icon">Jardí</p>
		<p class = "feature-description"> Descansa a la bora del nostre til·ler</p>
		<p class = "features"> <img src = "images/terraza.png" alt = "terrassa" class = "little-icon">Terrassa </p>
		<p class = "feature-description"> Disfruta de les vistes dels Rasos de Peguera i la Serra d'Ensija </p>
		<p class = "features"> <img src = "images/2bed.svg" alt = "2bed" class = "little-icon">2 llits de matrimoni</p>
		<p class = "features"> <img src = "images/bed.png" alt = "bed" class = "little-icon">Un llit individual </p> 
		<p class = "features"> <img src = "images/kitchen.png" alt = "cuina" class = "little-icon">Cuina </p> 
		<p class = "feature-description"> Totalment equipada. Microones. Forn. Nevera. Rentabaixelles </p>

		<hr />
		<p >El Jardinet és una caseta ubicada Borredà; un petit però marevellós municipi de muntanya situat a la comarca del Berguedà.</p>
		<hr />
		<!-- <Album /> -->
		<p> Seguiu-nos a instagram a <a href="https://instagram.com/eljardinetdeborreda" alt="">@eljardinetdeborreda</a> per a veure més fotografies i no perdreus cap novetat!</p>
	</div>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
		font-family: 'Titillium Web', sans-serif;
	}
	
	.features {
		font-size: 1.2em;
		font-weight: bold;

	}

	.little-icon {
		max-width: 15px;
		margin-right: 20px;
	}

	.feature-description {
		margin-left: 35px;
		margin-top: -20px
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}

	hr {
    display: block;
    height: 1px;
    border: 0;
    border-top: 1px solid #ccc;
    margin: 1em 0;
    padding: 0;
}
</style>