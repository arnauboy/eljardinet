<script>
  // import album from "./albumLoader.js"
</script>

<h1> Àlbum de fotos </h1>

<section class="gallery">
    <div class="gallery__item">
      <input type="radio" id="img-1" checked name="gallery" class="gallery__selector"/>
      <img class="gallery__img" src="images/album/convidats.JPG" alt="convidats"/>
      <label for="img-1" class="gallery__thumb"><img src="images/album/convidats.JPG" alt=""/></label>
    </div>
    <div class="gallery__item">
      <input type="radio" id="img-2" checked name="gallery" class="gallery__selector"/>
      <img class="gallery__img" src="images/album/cuina.JPG" alt="cuina"/>
      <label for="img-2" class="gallery__thumb"><img src="images/album/cuina.JPG" alt=""/></label>
    </div>
    <div class="gallery__item">
      <input type="radio" id="img-3" checked name="gallery" class="gallery__selector"/>
      <img class="gallery__img" src="images/album/habitacio_gran.JPG" alt="habitacio gran"/>
      <label for="img-3" class="gallery__thumb"><img  src="images/album/habitacio_gran.JPG" alt=""/></label>
    </div>
    <div class="gallery__item">
      <input type="radio" id="img-4" checked name="gallery" class="gallery__selector"/>
      <img class="gallery__img" src="images/album/lavabo.JPG" alt="lavabo"/>
      <label for="img-4" class="gallery__thumb"><img  src="images/album/lavabo.JPG" alt=""/></label>
    </div>
    <div class="gallery__item">
      <input type="radio" id="img-5" checked name="gallery" class="gallery__selector"/>
      <img class="gallery__img" src="images/album/menjador.JPG" alt="menjador"/>
      <label for="img-5" class="gallery__thumb"><img  src="images/album/menjador.JPG" alt=""/></label>
    </div>
    <div class="gallery__item">
      <input type="radio" id="img-6" checked name="gallery" class="gallery__selector"/>
      <img class="gallery__img" src="images/album/petita.JPG" alt="petita"/>
      <label for="img-6" class="gallery__thumb"><img  src="images/album/petita.JPG" alt=""/></label>
    </div>
    <div class="gallery__item">
      <input type="radio" id="img-7" checked name="gallery" class="gallery__selector"/>
      <img class="gallery__img" src="images/album/sencera.JPG" alt="sencera"/>
      <label for="img-7" class="gallery__thumb"><img  src="images/album/sencera.JPG" alt=""/></label>
    </div>
    <div class="gallery__item">
      <input type="radio" id="img-8" checked name="gallery" class="gallery__selector"/>
      <img class="gallery__img" src="images/album/sofa.JPG" alt="sofa"/>
      <label for="img-8" class="gallery__thumb"><img  src="images/album/sofa.JPG" alt=""/></label>
    </div>
    <div class="gallery__item">
      <input type="radio" id="img-9" checked name="gallery" class="gallery__selector"/>
      <img class="gallery__img" src="images/album/terrassa.JPG" alt="terrassa"/>
      <label for="img-9" class="gallery__thumb"><img  src="images/album/terrassa.JPG" alt=""/></label>
    </div>
    <div class="gallery__item">
      <input type="radio" id="img-10" checked name="gallery" class="gallery__selector"/>
      <img class="gallery__img" src="images/album/terrassa2.JPG" alt="terrassa2"/>
      <label for="img-10" class="gallery__thumb"><img  src="images/album/terrassa2.JPG" alt=""/></label>
    </div>
</section>

<style lang="scss">

    * {
    box-sizing: border-box;
    }

    $max-img-width: 600px;
    $max-img-height: 400px;

    img {
    max-width: 80%;
    vertical-align: top;
    }

    .gallery {
        display: flex;
        margin: 10px auto;
        max-width: $max-img-width;
        position: relative;
        padding-top: calc($max-img-height/$max-img-width) * 100%;
          
        @media screen and (min-width: $max-img-width){
        padding-top: $max-img-height;
        }
    
        &__img {
            position: absolute;
            top: 0;
            left: 55px;
            opacity: 0;
            transition: opacity 0.3s ease-in-out;
            box-shadow: rgb(38, 57, 77) 0px 20px 30px -10px;        }
        
        &__thumb {
            display: block;
        }
        
        &__selector {
            position: absolute;
            opacity: 0;
            visibility: hidden;
            
            &:checked {
            + .gallery__img {
                opacity: 1;
            }
            ~ .gallery__thumb > img {
                box-shadow: 0 0 0 3px #0be2f6;;
            }
            }
        }
    
    
    }
</style>