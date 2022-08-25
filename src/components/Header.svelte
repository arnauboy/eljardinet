<script>
    import Back from "./Back.svelte";
    import BookButton from "./BookButton.svelte";
    import ContactButton from "./ContactButton.svelte";
    export let route;

    function changeCss () {
        var bodyElement = document.querySelector("body");
        var bookButton = document.querySelector("book_button");
        this.scrollY > 100 ? bookButton.style.visibility = visible : bookButton.style.visibility = hidden;
    }
    window.addEventListener("book_button", changeCss , false);
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
     }

     #book_button {
        float:left;
     }

     @media (max-width: 750px) {

        .header-buttons {
            padding: 5px;   
        }
	}
</style>