<script>
  export let segment;

  let current = segment;
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
    /*padding-right: 20px;*/
    margin-right: 25px;
    padding-bottom: 5px;
  }

  .isLink:hover {
    color: darkgray;
    /*font-weight: inherit;*/
    cursor: pointer;
    border-bottom: solid 1px #ff1d1d;/*site colo*/
  }

  .selected {
    /*color: darkgray;*/
    /*font-weight: 500;*/
    border-bottom: solid 1px #ff1d1d;/*site colo*/
  }
</style>

<nav>
  <h2 class="title siteColor">projects</h2>
  <a  class="isLink" class:selected='{segment === "all"}' href='all'>
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
  </a>
</nav>
