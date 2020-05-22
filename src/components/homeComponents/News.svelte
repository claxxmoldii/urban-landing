<script type="text/javascript">

</script>

<style type="text/css">
  section {
    background-color: white;
    /*background-color: lightcyan;*/
  }

  .isLatestNews {
    height: 60vh;
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    align-items: center;
  }

  header {
    order: 2;
    cursor: pointer;
  }

  h1, h4 {
    font-family: 'Open Sans', 'Raleway', sans-serif;
  }

  h4 {
    font-weight: 600;
  }

  h4, p {
    margin: 0;
  }

  header div {
    height: 200px;
  }

  header h1 {
    font-size: 1.5rem;
    font-weight: 700;
    line-height: 1.5rem;
    margin: 0;
  }

  header .isBigger {
    font-size: 2.5rem;
    line-height: 2.5rem;
  }

  span.textOutlineFx {
    text-shadow:
      -.5px -.5px 0 #ff1d1d,
      .5px -.5px 0 #ff1d1d,
      -.5px .5px 0 #ff1d1d,
      .5px .5px 0 #ff1d1d;
  }

  .isAwards {
    order: 1;
    cursor: pointer;
    /*background-color: beige;*/
  }

  .isArchitravel {
    order: 3;
    cursor: pointer;
  }

  img {
    height: 200px;
    width: auto;
  }

  p {
    font-size: .9rem;
  }
</style>

<section class="isLatestNews">
  <header>
    <div>
      <h1 class="siteColor">
        We are <br>
        <span class="isBigger">confined</span> <br>
        but not <br>
        <span class="isBigger textOutlineFx">disconnected</span>
      </h1>
    </div>
    <h4>we're stil working and available</h4>
    <p class="isDate">18.03.2020</p>
  </header>
  <div class="isAwards">
    <img class="imejii" src="./images/publicaAwards.jpg" alt="nice award!">
    <h4>We're nominated for the Publica Awards </h4>
    <p class="isDate">24.03.2020</p>
  </div>
  <div class="isArchitravel">
    <img class="imejii" src="./images/architravel.jpg" alt="nice article!">
    <h4>We're nominated for the Publica Awards </h4>
    <p class="isDate">02.03.2020</p>
  </div>
</section>
