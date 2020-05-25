<style type="text/css">
  section {
    display: grid;
    grid-template-rows: [isCreative] 250px
                        [isPlayful] 250px
                        [pic1] 400px
                        [break] 100px
                        [isEfficient] 250px
                        [isSustainable] 250px
                        [pic2] 400px;
  }

  .isDefinition {
    height: 200px;
    /*background-color: lightcyan;*/
    /*border: solid crimson 1px;*/
  }

  p {
    font-size: 0.9rem;
  }

  span {
    font-weight: 700;
  }

  .picHolder {
    width: 400px;
    height: 400px;
  }

  img {
    width: 100%;
    height: auto;
  }

  .isCreative {
    grid-area: isCreative;
  }

  .isPlayful {
    grid-area: isPlayful;
  }

  .pic1 {
    grid-area: pic1;
  }

  .break {
    grid-area: break;
  }

  .isEfficient {
    grid-area: isEfficient;
  }

  .isSustainable {
    grid-area: isSustainable;
  }

  .pic2 {
    grid-area: pic2;
  }
</style>

<section>
  <div class="isDefinition isCreative">
    <p>
      <span>Creative</span> and driven by curiosity, we always pursue innovative ideas in relation to projects but also in organizational terms. At the same time, we perform our duties rigorously and with a profound sense of <span>responsibility</span>.
    </p>
  </div>
  <div class="isDefinition isPlayful">
    <p>
      We share a positive and infectious sense of enthusiasm that is essential to the <span>pleasure</span> we take in the work we do. But we also focus on efficiency and <span>profitability</span>, keeping within project deadlines and budgets.
    </p>
  </div>

  <div class="picHolder pic1">
    <img src="images/26-1.jpg" alt="one on one meeting">
  </div>

  <div class="break"></div>

  <div class="isDefinition isEfficient">
    <p>
      Respect, honesty and goodwill are key elements in our attitude to people and projects. They are part of our sense of <span>integrity</span>. We also emphasize the need to listen and to assist in a spirit of <span>solidarity</span>.
    </p>
  </div>
  <div class="isDefinition isSustainable">
    <p>
      We believe that design is of the utmost importance to draw attention to strategic projects. That is why we continuously challenge a strictly ‘technical’ approach and why we transcend the functional and sustainable aspects of our projects.
    </p>
  </div>

  <div class="picHolder pic2">
    <img src="images/23-1.jpg" alt="office space">
  </div>
</section>
