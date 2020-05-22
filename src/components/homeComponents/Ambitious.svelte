<script type="text/javascript">
  let isImejii = './images/6.jpg';
</script>

<style type="text/css">
  section {
    background-color: white;
    /*background-color: lightcyan;*/
  }

  .isAmbitious {
    height: 70vh;
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    align-items: center;
  }

  header {
    order: 2;
    /*background-color: beige;*/
  }

  header h1 {
    font-family: 'Open Sans', 'Raleway', sans-serif;
    font-size: 1.7rem;
    font-weight: 700;
    margin: 0;
  }

  span.textOutlineFx {
    text-shadow: -.5px -.5px 0 #ff1d1d, .5px -.5px 0 #ff1d1d, -.5px .5px 0 #ff1d1d, .5px .5px 0 #ff1d1d;
  }

  .isBigger {
    font-size: 3.5rem;
  }

  .isImage {
    /*background-color: floralwhite;*/
  }

  .isImage {
    order: 1;
  }

  .imejii {
    height: 60vh;
    width: auto;
  }
</style>

<section class="isAmbitious">
  <header>
    <h1 class="siteColor">
      We are <br>
      <span class="isBigger">ambitious</span> <br>
      but not <br>
      <span class="isBigger textOutlineFx">pretentious</span>
    </h1>
  </header>
  <div class="isImage">
    <img class="imejii"
     src="./images/6.jpg"
     alt="nice building!">
  </div>
</section>
