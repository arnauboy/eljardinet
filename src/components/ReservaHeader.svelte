<script>
    import BookButton from "./BookButton.svelte";
    import BookingButton from "./BookingButton.svelte";
</script>

<div style="display: flex; margin: 0 auto; max-width: 80%; padding-top: 100px">
    <img src="../../images/house_edit.JPG" alt="El Jardinet" style="float:left; max-width: 70%;"/> 
    <div class="photo_box" style="float: right;  margin: 0 auto;  padding-top: 50px; ">
        <h1>El Jardinet de Borredà</h1>
        <p>Carrer doctor Vilardell 17, 08619 Borredà, Espanya </p>
        <p> 5 hostes · 3 dormitoris · 3 llits · 1 lavabo </p>
        <BookButton />
        <BookingButton />
    </div>
</div>

<style>
    p {
       margin-bottom: 30px;
    }

    img {
        border-radius: 15px;
    }

    .little-icon {
		max-width: 25px;
	}
</style>