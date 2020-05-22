<script type="text/javascript">
  import { onMount } from 'svelte';
  import { fade } from 'svelte/transition';

  let visibleS1 = true;
  let visibleS2 = false;
  let visibleS3 = false;
  let visibleS4 = false;
  let visibleS5 = false;
  let visibleS6 = false;
  let visibleS7 = false;
  let visibleS8 = false;

  let placeHolderPic = 'images/oldSofa.jpg'

  let slide01 = 'imagesGallery/1.jpg';
  let slide02 = 'imagesGallery/2.jpg';
  let slide03 = 'imagesGallery/3.jpg';
  let slide04 = 'imagesGallery/4.jpg';
  let slide05 = 'imagesGallery/5.jpg';
  let slide06 = 'imagesGallery/6.jpg';
  let slide07 = 'imagesGallery/7.jpg';
  let slide08 = 'imagesGallery/8.jpg';

  onMount(async () => {
    fadeS1();
    // setInterval(function() {
    //   fadeS1();
    // }, (5000*8));
  });

  const fadeS1 = () => {
    setTimeout(function() {
      visibleS1 = false;
      visibleS2 = true;
      fadeS2();
    }, 5000);
  }

  const fadeS2 = () => {
    setTimeout(function() {
      visibleS2 = false;
      visibleS3 = true;
      fadeS3();
    }, 5000);
  }

  const fadeS3 = () => {
    setTimeout(function() {
      visibleS3 = false;
      visibleS4 = true;
      fadeS4();
    }, 5000);
  }

  const fadeS4 = () => {
    setTimeout(function() {
      visibleS4 = false;
      visibleS5 = true;
      fadeS5();
    }, 5000);
  }

  const fadeS5 = () => {
    setTimeout(function() {
      visibleS5 = false;
      visibleS6 = true;
      fadeS6();
    }, 5000);
  }

  const fadeS6 = () => {
    setTimeout(function() {
      visibleS6 = false;
      visibleS7 = true;
      fadeS7();
    }, 5000);
  }

  const fadeS7 = () => {
    setTimeout(function() {
      visibleS7 = false;
      visibleS8 = true;
      fadeS8();
    }, 5000);
  }

  const fadeS8 = () => {
    setTimeout(function() {
      visibleS8 = false;
      visibleS1 = true;
      fadeS1();
    }, 5000);
  }
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
    grid-area: window;
  }
</style>

<div class="carousel">
  <!-- placeholder -->
  <!-- <div class="bgImgFx" style="background-image: url({placeHolderPic});"></div> -->
  {#if visibleS8}
    <div class="bgImgFx" transition:fade style="background-image: url({slide08});"></div>
  {/if}
  {#if visibleS7}
    <div class="bgImgFx" transition:fade style="background-image: url({slide07});"></div>
  {/if}
  {#if visibleS6}
    <div class="bgImgFx" transition:fade style="background-image: url({slide06});"></div>
  {/if}
  {#if visibleS5}
    <div class="bgImgFx" transition:fade style="background-image: url({slide05});"></div>
  {/if}
  {#if visibleS4}
    <div class="bgImgFx" transition:fade style="background-image: url({slide04});"></div>
  {/if}
  {#if visibleS3}
    <div class="bgImgFx" transition:fade style="background-image: url({slide03});"></div>
  {/if}
  {#if visibleS2}
    <div class="bgImgFx" transition:fade style="background-image: url({slide02});"></div>
  {/if}
  {#if visibleS1}
    <div class="bgImgFx" transition:fade style="background-image: url({slide01});"></div>
  {/if}
</div>

<!-- from bad to best! yeah! did it myself with svelte! -->



