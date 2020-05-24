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
    text-decoration: none;
    /*padding-right: 20px;*/
    margin-right: 25px;
    padding-bottom: 5px;
  }

  .isLink:hover {
    color: darkgray;
    /*font-weight: inherit;*/
    cursor: pointer;
  }

  .selected {
    /*color: darkgray;*/
    /*font-weight: 500;*/
    border-bottom: solid 1px #ff1d1d;/*site colo*/
  }
</style>

<nav>
  <h2 class="title siteColor">practice</h2>
  <a  class="isLink" class:selected='{segment === "current"}' href='practice'>
    platforms
  </a>
  <a  class="isLink" class:selected='{segment === "values"}' href='values'>
    values
  </a>
</nav>
