<script>
  // import album from "./albumLoader.js"
</script>

<h1> Àlbum de fotos </h1>

<section class="gallery">
  {#each album as foto, id }
    <div class="gallery__item">
      <input type="radio" id={id} checked name="gallery" class="gallery__selector"/>
      <img class="gallery__img" src="{foto}" alt=""/>
      <label for="img-1" class="gallery__thumb"><img src="https://picsum.photos/id/1015/150/100.jpg" alt=""/></label>
    </div>
  {/each}
</section>

<style lang="scss">

    * {
    box-sizing: border-box;
    }

    $max-img-width: 600px;
    $max-img-height: 400px;

    img {
    max-width: 100%;
    vertical-align: top;
    }

    .gallery {
    display: flex;
        margin: 10px auto;
        max-width: $max-img-width;
        position: relative;
        padding-top: $max-img-height/$max-img-width * 100%;
        
        @media screen and (min-width: $max-img-width){
        padding-top: $max-img-height;
        }
    
        &__img {
            position: absolute;
            top: 0;
            left: 0;
            opacity: 0;
            transition: opacity 0.3s ease-in-out;
        }
        
        &__thumb {
            padding-top: 6px;
            margin: 6px;
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