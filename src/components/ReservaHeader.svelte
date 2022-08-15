<script>
    import BookButton from "./BookButton.svelte";
    import BookingButton from "./BookingButton.svelte";
</script>

<div class="section">
    <div class = "background_image">
        <div class = "info_box">
            <h1>el Jardinet</h1>
            <a style = "text-decoration: none;"href= "https://www.google.es/maps/place/Carrer+Dr.+Miquel+Vilardell+i+Picas,+17,+08619+Borred%C3%A0,+Barcelona/@42.1346738,1.9911864,17z/data=!3m1!4b1!4m5!3m4!1s0x12a511fbfba3604f:0x2d1170643f95d03c!8m2!3d42.1346698!4d1.9933751?hl=ca">Carrer doctor Vilardell 17, Borredà, Espanya </a>
            <p style = "font-weight: bold"> 5 hostes · 3 dormitoris · 1 lavabo </p>
            <BookButton />
            <BookingButton />
        </div>
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
        background-size: cover;
        background-repeat: no-repeat;
        max-width: 70%;
        margin: 0 auto; 
        margin-top: 100px;
        background-position: center;
    }

    .info_box {
        margin-top: 10px; 
        margin-bottom: 10px; 
        margin-right: 650px; 
        background: rgba(255, 255, 255, .9); 
        border-radius: 10px; 
        padding: 10px; 
        max-width: 20%;  
        display:inline-block;
    }

    @media (max-width: 750px) {
        .background_image {
        background-image: none;
        max-width: 70%;
        margin: 0 auto; 
        
        }
        .info_box {
            background-color: rgb(101,198,110,0.4); 
            border-radius: 10px; 
            padding: 10px; 
            max-width: 100%;  
            margin: 0 auto;

        }
    }
</style>