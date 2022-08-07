<script>
    import BookButton from "./BookButton.svelte";
    import BookingButton from "./BookingButton.svelte";
</script>


<div class = "background_image">
    <div style="margin-top: -620px; margin-left: 60px; background: rgba(255, 255, 255, .9) ; border-radius: 10px; padding: 15px; width: 20%;">
        <h1>el Jardinet</h1>
        <a style = "text-decoration: none; color: black"href= "https://www.google.es/maps/place/Carrer+Dr.+Miquel+Vilardell+i+Picas,+17,+08619+Borred%C3%A0,+Barcelona/@42.1346738,1.9911864,17z/data=!3m1!4b1!4m5!3m4!1s0x12a511fbfba3604f:0x2d1170643f95d03c!8m2!3d42.1346698!4d1.9933751?hl=ca">Carrer doctor Vilardell 17, Borredà, Espanya </a>
        <p style = "font-weight: bold"> 5 hostes · 3 dormitoris · 1 lavabo </p>
        <BookButton />
        <BookingButton />
    </div>
</div>

<style>
    p {
       margin-bottom: 30px;
    }

    h1 {
        font-size: 30px;
    }

    .background_image {
        background-image: url("../images/house_edit.JPG");
        background-size: contain;
        background-repeat: no-repeat;
        max-width: 70%;
        margin: 0 auto; 
        height: 0px;
        padding-top: 38.65%;  /* (img-height / img-width * container-width); % - specifies a padding in % of the width of the containing element */ 
        margin-bottom: -200px;
    }

</style>