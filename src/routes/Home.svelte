<script>
    import Header from '../components/Header.svelte';
    import Icons from '../components/Icons.svelte';
	import ReservaHeader from '../components/ReservaHeader.svelte';
	import Album from '../components/Album.svelte';
	import Description from '../components/Description.svelte';
	import Installacions from '../components/Installacions.svelte';
	import Location from '../components/Location.svelte';
	import { scrollTo, scrollRef, scrollTop } from 'svelte-scrolling'
</script>

<svelte:head>
	<title>El Jardinet</title>
</svelte:head>


<Header route="/"/>
<Icons />
<ReservaHeader />
<!-- svelte-ignore a11y-invalid-attribute -->
<a use:scrollTo={{ ref: 'home_page', duration: 1000 }} href="#" class="scroll-down"> </a>
<div class="home_page"  use:scrollRef={'home_page'}>
	<Description />
	<hr />	
	<Installacions />
	<hr />
	<Location />
	<hr />
	<Album />
	<p style = "font-size: 1.2em; padding-bottom: 100px; padding-top: 100px;"> Seguiu-nos a instagram a <a href="https://instagram.com/eljardinetdeborreda" alt="">@eljardinetdeborreda</a> per a veure més fotografies i no perdreus cap novetat!</p>
</div>


<style>
	.home_page {
		max-width: 50%; text-align: left; margin: auto; margin-top: 50px;
	}

	.scroll-down {
		opacity: 1;
		-webkit-transition: all .5s ease-in 3s;
		transition: all .5s ease-in 3s;
		}

	.scroll-down {
		position: absolute;
		bottom: 30px;
		left: 50%;
		margin-left: -16px;
		display: block;
		width: 32px;
		height: 32px;
		border: 2px solid #FFF;
		background-size: 14px auto;
		border-radius: 50%;
		z-index: 2;
		-webkit-animation: bounce 2s infinite 2s;
		animation: bounce 2s infinite 2s;
		-webkit-transition: all .2s ease-in;
		transition: all .2s ease-in;
		}

	.scroll-down:before {
		position: absolute;
		top: calc(50% - 8px);
		left: calc(50% - 6px);
		transform: rotate(-45deg);
		display: block;
		width: 12px;
		height: 12px;
		content: "";
		border: 2px solid white;
		border-width: 0px 0 2px 2px;
		}

		@keyframes bounce {
			0%,
			100%,
			20%,
			50%,
			80% {
				-webkit-transform: translateY(0);
				-ms-transform: translateY(0);
				transform: translateY(0);
			}
			40% {
				-webkit-transform: translateY(-10px);
				-ms-transform: translateY(-10px);
				transform: translateY(-10px);
			}
			60% {
				-webkit-transform: translateY(-5px);
				-ms-transform: translateY(-5px);
				transform: translateY(-5px);
			}
		}

	@media (max-width: 600px){
		.home_page{
			max-width: 100%;
			text-align: justify;
			margin: 20px;
		}
	}

	@media (max-width: 1300px){
		.scroll-down{
			visibility: hidden;
		}
	}
</style>