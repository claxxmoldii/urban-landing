<script>
  export let segment;
</script>

<style type="text/css">
  nav {
    width: 100vw;
    padding: 30px 50px;
  }

  h2 {
    font-weight: 800;
  }

  a {
    font-size: .9rem;
    text-decoration: none;
    margin-right: 25px;
    padding-bottom: 5px;
  }

  a:hover {
    color: darkgray;
    cursor: pointer;
    border-bottom: solid 1px #ff1d1d;
  }

  [aria-current] {
    font-weight: 600;
    border-bottom: solid 1px #ff1d1d;
  }
</style>

{#if segment}
<nav>
  <h2 class="title siteColor">projects</h2>
  <a  aria-current='{segment === "all" ? "page" : undefined}'
      href='all'>
    all
  </a>
  <a  aria-current='{segment}'
      href='{segment}'>
    selected
  </a>
  <a  aria-current='{segment === "housing" ? "page" : undefined}'
      href='housing'>
    housing
  </a>
  <a  aria-current='{segment === "education" ? "page" : undefined}'
      href='education'>
    education
  </a>
  <a  aria-current='{segment === "urbanism" ? "page" : undefined}'
      href='urbanism'>
    urbanism
  </a>
  <a  aria-current='{segment === "mixedUse" ? "page" : undefined}'
      href='mixedUse'>
    mixed use
  </a>
  <a  aria-current='{segment === "butAlso" ? "page" : undefined}'
      href='butAlso'>
    but also
  </a>
</nav>
{/if}
