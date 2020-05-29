<script type="text/javascript">
  import * as animateScroll from "svelte-scrollto";

  import NavAbout from '../components/navComponents/NavAbout.svelte';
  import AboutPartners from '../components/aboutComponents/AboutPartners.svelte';
  import AboutTeam from '../components/aboutComponents/AboutTeam.svelte';
  import AboutCareers from '../components/aboutComponents/AboutCareers.svelte';
  import AboutContact from '../components/aboutComponents/AboutContact.svelte';

  function gotoContact() {
    animateScroll.scrollTo({element: '#contact', offset: -150, duration: 1500});
  }

  function gotoCareers() {
    animateScroll.scrollTo({element: '#careers', offset: -150, duration: 1000});
  }

  function gotoTeam() {
    animateScroll.scrollTo({element: '#team', offset: -150, duration: 500});
  }

  function gotoPartners() {
    animateScroll.scrollTo({element: '#partners', offset: -150, duration: 1000});
  }

  function yeah() {
    alert('yeah! yeah!');
  }

</script>

<style type="text/css">
  section {
    max-width: calc(100vw-150px);
    padding-bottom: 50px;
    overflow-x: hidden;
  }

  nav {
    position: fixed;
    background-color: #fff;
    z-index: 100;
  }

  main {
    min-height: 100vh;
    padding-top: 150px;
    display: grid;
    grid-template-columns: 1fr;
    grid-template-rows: [partners] auto [team] auto [careers] auto [contact] auto;

    scroll-behavior: smooth;
  }

  .aboutPartners {
    grid-row: partners;
  }

  .aboutTeam {
    grid-row: team;
  }

  .aboutCareers {
    grid-row: careers;
  }

  .aboutContact {
    grid-row: contact;
  }
</style>

<svelte:head>
	<title>About</title>
</svelte:head>

<section>
  <nav>
    <NavAbout segment={'about'}
              on:scrollToContact={gotoContact}
              on:scrollToCareers={gotoCareers}
              on:scrollToTeam={gotoTeam}
              on:scrollToPartners={gotoPartners}
    />
  </nav>
  <main>
    <div id="partners" class="aboutPartners">
      <AboutPartners />
    </div>
    <div id="team" class="aboutTeam">
      <AboutTeam />
    </div>
    <div id="careers" class="aboutCareers">
      <AboutCareers />
    </div>
    <div id="contact" class="aboutContact">
      <AboutContact />
    </div>
  </main>
</section>

