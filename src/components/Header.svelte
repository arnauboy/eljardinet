<script>
    import Back from "./Back.svelte";
    import BookButton from "./BookButton.svelte";
    import ContactButton from "./ContactButton.svelte";
    export let route;
</script>

<div class="header"> 
    <div class = "header-title">
        <!-- svelte-ignore missing-declaration -->
        <img src = "images/title.png" alt = "title"/>
    </div>
    <div class = "header-buttons">
        {#if route==="/"}
            <BookButton />
            <ContactButton />
        {:else}
            <Back />
        {/if}
        
    </div>
</div>


<style>
     .header {
        position: fixed;
        top: 0;
        width:100%; 
        background-color: white;
        display: flex;
    
     }

     .header-buttons {
        margin-left: auto;
        padding: 20px;
        width: 50%;
        
     }

     .header-title {
        margin-top: 20px;
        margin-left: -40px;
        margin: auto;
        width: 50%;
     }

     @media (max-width: 750px) {
		.header {
    	display: contents;
  		}

        .header-title {
            margin: 0 auto;
            width: 100%;
        }

        .header-buttons {
            margin: 0 auto;
            width: 100%;
            padding: 0;
        }
	}
</style>