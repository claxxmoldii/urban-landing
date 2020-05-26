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
  <h2 class="title siteColor">about</h2>
  <a  aria-current='{segment === "about" ? "page" : undefined}' href='about'>partners</a>
  <a  aria-current='{segment === "team" ? "page" : undefined}' href='team'>team</a>
  <a  aria-current='{segment === "careers" ? "page" : undefined}' href='careers'>careers</a>
  <a  aria-current='{segment === "contact" ? "page" : undefined}' href='contact'>contact</a>
</nav>
{/if}
