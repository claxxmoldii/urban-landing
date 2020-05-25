<script>
  // import NavPractice from '../components/navComponents/NavPractice.svelte';
  import Titles from 'Titles.svelte';
  import Definitions from 'Definitions.svelte';
  import FauxArrow from 'FauxArrow.svelte';
</script>

<style type="text/css">
  main {
    position: relative;
  }

  nav {
    position: fixed;
    /*background-color: beige;*/
    background-color: #fff;
    z-index: 100;
  }

  main {
    padding: 0 50px;
    padding-top: 150px;
    display: grid;
    grid-template-columns: [titles] 4fr [arrow] 2fr [definitions] 4fr;
    /*background-color: lightcyan;*/
  }

  .isTitles {
    grid-area: titles;
  }

  .isDefinitions {
    grid-area: definitions;
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
	<title>Practice/Values</title>
</svelte:head>

<main>
  <div class="isTitles">
    <Titles />
  </div>
  <div class="isDefinitions">
    <Definitions />
  </div>
  <div class="divider">
    <FauxArrow />
  </div>
</main>

<!-- <section>
  <nav>
    <NavPractice segment={'values'}/>
  </nav>
  <main>
    <div class="isTitles">
      <Titles />
    </div>
    <div class="isDefinitions">
      <Definitions />
    </div>
    <div class="divider">
      <FauxArrow />
    </div>
  </main>
  <footer></footer>
</section> -->
