<script>
  // import NavPractice from '../components/navComponents/NavPractice.svelte';
  import Design from '../components/practiceComponents/Design.svelte';
  import Planning from '../components/practiceComponents/Planning.svelte';
  import FauxArrow from '../components/practiceComponents/FauxArrow.svelte';
</script>

<style type="text/css">
  main {
    position: relative;
    padding: 0 50px;
    padding-top: 150px;
    display: grid;
    grid-template-columns: [design] 4fr [arrow] 2fr [planning] 4fr;
    /*background-color: lightcyan;*/
  }

  nav {
    position: fixed;
    /*background-color: beige;*/
    background-color: #fff;
    z-index: 100;
  }

  .isDesign {
    grid-area: design;
  }

  .isPlanning {
    grid-area: planning;
  }

  .divider {
    grid-area: arrow;
    /*background-color: darkgrey;*/
    height: 100%;
    width: 100%;
  }

  footer {
    height: 60px;
    width: 100%;
    /*background-color: beige;*/
  }
</style>


<svelte:head>
  <title>Practice/Platform</title>
</svelte:head>

<main>
  <div class="isDesign">
    <Design />
  </div>
  <div class="isPlanning">
    <Planning />
  </div>
  <div class="divider">
    <FauxArrow />
  </div>
</main>

<!-- <section>
  <nav>
    <NavPractice segment={'practice'}/>
  </nav>
  <main>
    <div class="isDesign">
      <Design />
    </div>
    <div class="isPlanning">
      <Planning />
    </div>
    <div class="divider">
      <FauxArrow />
    </div>
  </main>
  <footer></footer>
</section> -->
