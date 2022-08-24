<script>
    import BookButton from "./BookButton.svelte";
    import BookingButton from "./BookingButton.svelte";
</script>

<div class="section">
    <div class = "background_image">
        <div class = "info_box">
            <div>
                <img src = "images/title.png" alt = "title"/>
            </div>
            <a id="maps_link" style = "text-decoration: none;"href= "https://www.google.es/maps/place/Carrer+Dr.+Miquel+Vilardell+i+Picas,+17,+08619+Borred%C3%A0,+Barcelona/@42.1346738,1.9911864,17z/data=!3m1!4b1!4m5!3m4!1s0x12a511fbfba3604f:0x2d1170643f95d03c!8m2!3d42.1346698!4d1.9933751?hl=ca">Carrer doctor Vilardell 17, Borredà, Espanya </a>
            <p style = "font-weight: bold"> 5 hostes · 3 dormitoris · Jardí · Terrassa</p>
            <BookButton />
            <BookingButton />
        </div>
    </div>
</div>

<style>
    p {
       margin-bottom: 30px;
    }

    .background_image {
        background-image: url("../images/house.JPG");
        background-size: cover;
        background-repeat: no-repeat;  
        background-position: center;
        padding-bottom: 20%;
        box-shadow: rgb(38, 57, 77) 0px 10px 10px -10px;
        display: flex;        
    }
    
    .info_box {
        background: rgba(255, 255, 255, .8); 
        padding: 10px; 
        max-width: 50%;  
        border-radius: 10px;
        margin-top: 15%;
        margin-left: 25%;
        float: left;
    }

    @media (max-width: 750px) {
        .info_box {
            border-radius: 10px; 
            padding: 10px; 
            max-width: 100%;  
            margin-top: 20%;
            margin-bottom: auto;
            margin-left: auto;
            margin-right: auto;
        }

        #maps_link {
            visibility: hidden;
        }
    }
</style>