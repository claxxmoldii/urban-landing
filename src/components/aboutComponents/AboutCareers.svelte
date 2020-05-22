<script type="text/javascript">
  import AboutJobs from './AboutJobs.svelte';

  const seniorArchitectNL = {
          job: 'senior architect NL',
          jobDescription: 'resolutely sympathetic'
        };

  const spontaneousApplication = {
          job: 'spontaneous application',
          jobDescription: 'apply now!'
        };

  const seniorArchitect = {
          job: 'senior architect',
          jobDescription: 'casually committed'
        };
</script>

<style type="text/css">
  section {
    padding-bottom: 50px;
  }

  h4 {
    font-family: 'Open Sans', 'Raleway', sans-serif;
    font-weight: 700;
    margin-bottom: 0;
    margin-left: 50px;
    padding-bottom: 10px;
  }

  main {
    min-height: 100vh;
    max-width: 100%;
    position: relative;
    padding: 0 50px;
  }

  main {
    display: grid;
    /*margin: 0 auto;*/
    grid-template-columns: 1fr 1fr;
    grid-auto-rows: minmax(275px, auto);
    column-gap: 20px;
    row-gap: 20px;
  }
</style>

<section>
  <h4 class="siteColor">we're looking for</h4>
  <main>
    <AboutJobs {...seniorArchitectNL}/>
    <AboutJobs {...spontaneousApplication}/>
    <AboutJobs {...seniorArchitect}/>
  </main>
</section>
