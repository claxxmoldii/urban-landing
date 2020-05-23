<script>
  import NavMain from '../components/navComponents/NavMain.svelte';
  import NavSecondary from '../components/navComponents/NavSecondary.svelte';
  import NavSapper from '../components/navComponents/NavSapper.svelte';
  import Footer from '../components/Footer.svelte';

  export let segment;
</script>

<style>
  .mainDiv {
    max-width: 100vw;
    display: grid;
    grid-template-columns: [nav] 150px [main-section] 1fr;
    font-family: 'Raleway', sans-serif;
  }

  nav {
    grid-column: nav;
    position: relative;
    border-right: solid .5px #dede;
  }

  .mainDiv nav div {
    position: fixed;
    left: 0;
    top: 0;
  }

  section {
    grid-column: main-section;
    display: grid;
    grid-template-rows: [navigation] auto [main] auto [footer] auto;
    position: relative;
  }

  section header {
    grid-row: navigation;
    display: block;
    position: fixed;
    background-color: white;
    z-index: 1000;
  }

  main {
    grid-row: main;
    min-height: 100vh;
  }

  footer {
    grid-row: footer;
  }
</style>

<div class="mainDiv">
  <nav>
    <div>
      <NavMain {segment}/>
    </div>
  </nav>
  <section>
    {#if segment !== undefined}
    <header><NavSecondary {segment}/></header>
    {/if}
    <main>
        <slot></slot>
    </main>
    <footer>
      <Footer />
    </footer>
  </section>
</div>
