<script type="text/javascript">
</script>

<style type="text/css">
  section {
    background-color: white;
    /*background-color: lightcyan;*/
  }

  .isHardWorking {
    height: 80vh;
    display: grid;
    grid-template-columns: [copy] 1fr [header] 1fr;
    align-items: start;
  }

  header {
    grid-area: header;
/*    margin: 0 auto;*/
    /*centering*/
    /*display: flex;
    justify-content: center;
    align-items: center;*/
    align-self: center;
    justify-self: center;
    padding-bottom: 50px;
    padding-left: 50px;
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
    text-shadow:
      -.5px -.5px 0 #ff1d1d,
       .5px -.5px 0 #ff1d1d,
      -.5px .5px 0 #ff1d1d,
       .5px .5px 0 #ff1d1d;
  }

  p {
    font-size: .9rem;
    padding: 0 140px;
  }

  .isCopy {
    grid-area: copy;

/*    padding-right: 0 140px;
    height: 80%;
    background-color: beige;
*/  }

  .isCopy div {
    border-right: solid 1px #ff1d1d;
    padding-right: 0 140px;
    height: 80%;
    /*background-color: beige;*/
  }
</style>

<section class="isHardWorking">
  <header>
    <h1 class="siteColor">
        We are <br>
        <span class="isBigger">hard-working</span> <br>
        but not <br>
        <span class=" isBigger textOutlineFx">hard-headed</span>
    </h1>
  </header>
  <div class="isCopy">
    <div>
      <p>
        Urban Platform is an architecture and urbanism practice. Founded in 2000, the office proposes a strong and innovative vision founded on analysis and design. Armed with excellent skills in project management, we have experience in both the public and private sectors.
      </p>
      <p>
        Thanks to our design expertise, we can bring a touch of magic to your projects. Conversely, the many buildings we have constructed have given us the experience necessary to translate your aspirations into a tangible reality.
      </p>
    </div>
  </div>
</section>
