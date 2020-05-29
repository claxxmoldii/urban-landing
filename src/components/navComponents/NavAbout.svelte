<script>
  import { createEventDispatcher } from 'svelte';

  const dispatch = createEventDispatcher();

  function gotoContact() {
    dispatch('scrollToContact');
  }

  function gotoCareers() {
    dispatch('scrollToCareers');
  }

  function gotoTeam() {
    dispatch('scrollToTeam');
  }

  function gotoPartners() {
    dispatch('scrollToPartners');
  }

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
  <a  on:click={gotoPartners} aria-current='{segment === "about" ? "page" : undefined}'>partners</a>
  <a  on:click={gotoTeam} aria-current='{segment === "team" ? "page" : undefined}'>team</a>
  <a  on:click={gotoCareers} aria-current='{segment === "careers" ? "page" : undefined}'>careers</a>
  <a  on:click={gotoContact} aria-current='{segment === "contact" ? "page" : undefined}'>contact</a>
</nav>
{/if}
