<script type="text/javascript">
</script>

<style type="text/css">
  section {
    background-color: white;
  }

  .isIdealistic {
    height: 60vh;
    display: grid;
    grid-template-columns: [copy] 2fr [header] 1fr;
    align-items: start;
  }

  header {
    grid-area: header;
    display: flex;
    justify-content: center;
    align-items: center;
    padding-top: 50px;
    /*background-color: beige;*/
  }

  h3, p {
    margin: 0;
    padding: 0;
  }

  h3 {
    font-weight: 700;
    line-height: 2rem;
    /*padding-top: 15px;*/
    padding-left: 50px;
    height: 80px;
  }

  p {
    font-size: .9rem;
  }

  header h1 {
    font-family: 'Open Sans', 'Raleway', sans-serif;
    font-size: 1.7rem;
    font-weight: 700;
    margin: 0;
  }

  .isBigger {
    font-size: 3.5rem;
  }

  span.textOutlineFx {
    text-shadow: -.5px -.5px 0 #ff1d1d, .5px -.5px 0 #ff1d1d, -.5px .5px 0 #ff1d1d, .5px .5px 0 #ff1d1d;
  }

  .isCopy {
    height: 40vh;
    grid-area: copy;
    display: grid;
    grid-template-rows: [concept] 1fr [planning] 1fr;
  }

  .isCopy p {
    padding: 0 50px;
  }

  .isConcept {
    grid-area: concept;
    display: grid;
    grid-template-columns: [concept-title] 1fr [concept-description] 1fr;
    justify-content: center;
    /*background-color: beige;*/
  }

  .isConcept .isTitle {
    grid-area: concept-title;
    padding-top: 20px;
  }
  .isConcept .isDescription {
    grid-area: concept-description;
    padding-top: 20px;
  }

  .isPlanning {
    grid-area: planning;
    display: grid;
    grid-template-columns: [planning-title] 1fr [planning-description] 1fr;
    /*background-color: lightcyan;*/
  }

  .isPlanning .isTitle {
    grid-area: planning-title;
    padding-top: 20px;
  }
  .isPlanning .isDescription {
    grid-area: planning-description;
  }

  .fauxStuff {
    display: block;
    width: 60%;
    padding-bottom: 34px;
    border-bottom: solid 1px #333;
  }
</style>

<section class="isIdealistic">
  <header>
    <h1 class="siteColor">
      We are <br>
      <span class="isBigger">idealistic</span> <br>
      but not <br>
      <span class="isBigger textOutlineFx">unrealistic</span>
    </h1>
  </header>
  <div class="isCopy">
    <div class="isConcept">
      <h3 class="isTitle">
        Concept & <br>
        Architectural design
        <span class="fauxStuff"></span>
      </h3>
      <p class="isDescription">
        Platform 1 concentrates on a wide range of sustainable architecture projects supported by an ambitious creative vision.
      </p>
    </div>
    <div class="isPlanning">
      <h3 class="isTitle">
        Territorial & <br>
        Urban Planning
      </h3>
      <p class="isDescription">
        Platform 2 concentrates on a wide range of sustainable architecture projects supported by an ambitious creative vision.
      </p>
    </div>
  </div>
</section>
