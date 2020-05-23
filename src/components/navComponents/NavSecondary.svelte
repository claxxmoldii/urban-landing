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

  .isLink:hover {
    color: darkgray;
    cursor: pointer;
    border-bottom: solid 1px #ff1d1d;/*site colo*/
  }

  .selected {
    border-bottom: solid 1px #ff1d1d;/*site colo*/
  }

  [aria-current] {
    font-weight: 600;
    border-bottom: solid 1px #ff1d1d;/*site colo*/
  }
</style>

{#if segment }
<nav>
  <h2 class="title siteColor">{segment}</h2>
  <a  class="isLink"
      aria-current='{segment === "all" ? "page" : undefined}'
      href='all'>
    all
  </a>
  <a  class="isLink"
      aria-current='{segment === "projects" ? "page" : undefined}'
      href='{segment}'>
    {segment}
  </a>
  <a  class="isLink"
      aria-current='{segment === "housing" ? "page" : undefined}'
      href='housing'>
    housing
  </a>
  <a  class="isLink"
      aria-current='{segment === "education" ? "page" : undefined}'
      href='education'>
    education
  </a>
  <a  class="isLink"
      aria-current='{segment === "urbanism" ? "page" : undefined}'
      href='urbanism'>
    urbanism
  </a>
  <a  class="isLink"
      aria-current='{segment === "mixedUse" ? "page" : undefined}'
      href='mixedUse'>
    mixed use
  </a>
  <a  class="isLink"
      aria-current='{segment === "butAlso" ? "page" : undefined}'
      href='butAlso'>
    but also
  </a>
</nav>
{/if}
<!-- <a  class="isLink" class:selected='{segment === "all"}' href='all'>
    all
  </a>
  <a  class="isLink" class:selected='{segment === current}' href='selected'>
    selected
  </a>
  <a  class="isLink" class:selected='{segment === "housing"}' href='housing'>
    housing
  </a>
  <a  class="isLink" class:selected='{segment === "education"}' href='education'>
    education
  </a>
  <a  class="isLink" class:selected='{segment === "urbanism"}' href='urbanism'>
    urbanism
  </a>
  <a  class="isLink" class:selected='{segment === "mixedUse"}' href='mixedUse'>
    mixed use
  </a>
  <a  class="isLink" class:selected='{segment === "butAlso"}' href='butAlso'>
    but also
  </a> -->
