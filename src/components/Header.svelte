<script>
    import BookButton from "./BookButton.svelte";
    import ContactButton from "./ContactButton.svelte";
</script>

<div class="header"> 
    <div>
        <BookButton />
        <ContactButton />
    </div>
    
</div>


<style>
     .header {
        position: fixed;
        top: 0;
        width:100%; 
     }
     .header div {
        float:right;
        margin: 30px;
     }
</style>