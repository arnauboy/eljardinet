<script>
	import { Router, Link, Route } from "svelte-routing";
	import Book from "./routes/Book.svelte";
	import Contact from "./routes/contact.svelte";
	import Home from "./routes/Home.svelte"
	export let url = "";
</script>

<svelte:head>
	<title>El Jardinet</title>
	<link rel="preconnect" href="https://fonts.googleapis.com">
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
	<link href="https://fonts.googleapis.com/css2?family=Titillium+Web&display=swap" rel="stylesheet">
	<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
</svelte:head>

<main>
	<Router url="{url}">
		<div>
			<Route path="book" component="{Book}" />
			<Route path="contact" ><Contact /></Route>
			<Route path="/"><Home /></Route>
		</div>
	</Router>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
		font-family: 'Titillium Web', sans-serif;
		
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}

	:global(hr) {
    display: block;
    height: 1px;
    border: 0;
    border-top: 1px solid #65C66E;
    margin: 1em 0;
    padding: 0;
}
</style>

