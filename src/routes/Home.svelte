<script>
	import BookButton from './../components/BookButton.svelte';
    import Header from '../components/Header.svelte';
    import Icons from '../components/Icons.svelte';
</script>

<svelte:head>
	<title>El Jardinet</title>
</svelte:head>

<main>
	<Header />
    <Icons />
	<h1>El Jardinet De Borredà</h1>
	<h2> Una caseta de conte🏡</h2>
	<div>
		<BookButton />
	</div>
	<p class="description">El Jardinet és una caseta ubicada Borredà; un petit però marevellós municipi de muntanya situat a la comarca del Berguedà. </p>
	<p class="description">No us ho perdeu i gaudiu d'una inoblidable estada rural.</p>
	<p> Seguiu-nos a instagram a <a href="https://instagram.com/eljardinetdeborreda" alt="">@eljardinetdeborreda</a> per a veure més fotografies i no perdreus cap novetat!</p>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
		font-family: 'Titillium Web', sans-serif;
	}

	h1 {
		color: black;
		font-size: 4em;
		font-weight: bold;
	}

	h2 {
		color: black;
		font-size: 2em;
	}

	.description {
		font-size: 2em;

	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}

    .fa {
        padding: 20px;
        font-size: 30px;
        width: 30px;
        text-align: center;
        text-decoration: none;
        border-radius: 50%;
        }
    
    .fa-instagram {
        background: #125688;
        color: white;
        }
</style>