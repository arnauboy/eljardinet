<script>
    import BookButton from "./BookButton.svelte";
    import ContactButton from "./ContactButton.svelte";
</script>

<div class="header"> 
    <div class = "header-title">
        <img src = "images/title.png" alt = "title"/>
    </div>
    <div class = "header-buttons">
        <BookButton />
        <ContactButton />
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
</style>