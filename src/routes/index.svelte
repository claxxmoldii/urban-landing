<script type="text/javascript">
  import Seriously from '../components/homeComponents/Seriously.svelte';
  import Carousel from '../components/homeComponents/Carousel.svelte';
  import BgFx from '../components/homeComponents/BgFx.svelte';
  import HardWorking from '../components/homeComponents/HardWorking.svelte';
  import Idealistic from '../components/homeComponents/Idealistic.svelte';
  import News from '../components/homeComponents/News.svelte';
  import Ambitious from '../components/homeComponents/Ambitious.svelte';
</script>

<style>
  section {
    font-family: 'Raleway', sans-serif;
    display: grid;
  }

  .carousel {
    z-index: 50;
  }

  .isBanner {
    z-index: 100;
  }

  .isHardWorking,
  .isIdealistic,
  .isAmbitious,
  .isNews {
    z-index: 200;
  }

  @media (min-width: 480px) {
    h1 {
      font-size: 4em;
    }
  }
</style>

<svelte:head>
  <title>urban landing</title>
</svelte:head>

<section>
  <div class="isBanner">
    <Seriously />
  </div>
  <div class="carousel">
    <Carousel/>
  </div>
  <div class="isHardWorking">
    <HardWorking />
  </div>
  <BgFx />
  <div class="isIdealistic">
    <Idealistic />
  </div>
  <div class="isNews">
    <News />
  </div>
  <div class="isAmbitious">
    <Ambitious />
  </div>
</section>
