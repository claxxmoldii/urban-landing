<script type="text/javascript">
  import { onMount } from 'svelte';
  import { fade } from 'svelte/transition';

  let placeHolderPic = 'images/oldSofa.jpg';

  let visibleS1 = true;
  let visibleS2 = false;
  let visibleS3 = false;
  let visibleS4 = false;
  let visibleS5 = false;
  let visibleS6 = false;

  let visi = visibleS1;

  let slideDiv1;//svelte dom element binding
  let slideDiv2;//svelte dom element binding

  let slide01 = 'imagesGallery/1.jpg';
  let slide02 = 'imagesGallery/2.jpg';
  let slide03 = 'imagesGallery/3.jpg';
  let slide04 = 'imagesGallery/4.jpg';
  let slide05 = 'imagesGallery/5.jpg';
  let slide06 = 'imagesGallery/6.jpg';

  let url;

  const slides = [
    'imagesGallery/1.jpg',
    'imagesGallery/2.jpg',
    'imagesGallery/3.jpg',
    'imagesGallery/4.jpg',
    'imagesGallery/5.jpg',
    'imagesGallery/6.jpg'
  ];

  const switchie = (url) => {
    slideDiv.style.backgroundImage = `url(${url})`;
  }

  onMount(async () => {

  });
</script>

<style type="text/css">
  .carousel {
    display: grid;
    grid-template-columns: [window] 100%;
  }

  .bgImgFx {
    background: no-repeat center center;
    background-size: cover;
    height: 100vh;
    width: 100%;
    /*grid-area: window;*/
  }
</style>

<div class="carousel">
  <!-- placeholder -->
  <!-- <div class="bgImgFx" style="background-image: url({placeHolderPic});"></div> -->
  {#each slides as slide}
    <div  class="bgImgFx"
      transition:fade
      style="background-image: url({slide});">
    </div>
  {/each}

  <!-- {#if visibleS1}
    <div  class="bgImgFx"
          transition:fade
          style="background-image: url({slides[0]});">
    </div>
  {/if}
  {#if visibleS2}
    <div  class="bgImgFx"
          transition:fade
          style="background-image: url({slides[1]});">
    </div>
  {/if}
  {#if visibleS3}
    <div  class="bgImgFx"
          transition:fade
          style="background-image: url({slides[2]});">
    </div>
  {/if}
  {#if visibleS4}
    <div  class="bgImgFx"
          transition:fade
          style="background-image: url({slides[3]});">
    </div>
  {/if}
  {#if visibleS5}
    <div  class="bgImgFx"
          transition:fade
          style="background-image: url({slides[4]});">
    </div>
  {/if}
  {#if visibleS6}
    <div  class="bgImgFx"
          transition:fade
          style="background-image: url({slides[5]});">
    </div>
  {/if} -->
</div>



