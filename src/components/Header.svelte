<script>
    import Back from "./Back.svelte";
    import BookButton from "./BookButton.svelte";
    import ContactButton from "./ContactButton.svelte";
    export let route;
</script>

<div class="header"> 
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
        display: flex;
     }

     .header-buttons {
        margin-left: auto;
        padding: 20px;
        width: 50%;
        
     }

     @media (max-width: 750px) {

        .header-buttons {
            padding: 5px;
            width: 70%;
        }
	}
</style>