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

  .isTitle {
    height: 200px;
/*    background-color: beige;
    border: solid crimson 1px;*/
  }

  h1 {
    color: #ff1d1d;/*site colo*/
    font-family: 'Open Sans', 'Raleway', sans-serif;
    font-size: 1.4rem;
    font-weight: 700;
    padding-left: 25%
  }

  h1 span {
    font-size: 2.3rem;
    font-weight: 900;
  }

  .isOutlined {
    color: transparent;
    -webkit-text-stroke-width: 0.8px;
    -webkit-text-stroke-color: #ff1d1d;
  }

  .picHolder {
    width: 400px;
    height: 400px;
  }

  img {
    width: 100%;
    height: auto;
  }
</style>

<section>
  <div class="isTitle isCreative">
    <h1>
      We are<br/>
      <span>creative</span><br/>
      but<br/>
      <span class="isOutlined">precise</span>
    </h1>
  </div>
  <div class="isTitle isPlayful">
    <h1>
      We are<br/>
      <span>playful</span><br/>
      but<br/>
      <span class="isOutlined">practical</span>
    </h1>
  </div>

  <div class="picHolder pic1">
    <img src="images/26.jpg" alt="office space">
  </div>

  <div class="break"></div>

  <div class="isTitle isEfficient">
    <h1>
      We are<br/>
      <span>efficient</span><br/>
      but<br/>
      <span class="isOutlined">easy-going</span>
    </h1>
  </div>
  <div class="isTitle isSustainable">
    <h1>
      We are<br/>
      <span>sustainable</span><br/>
      but<br/>
      <span class="isOutlined">sociable</span>
    </h1>
  </div>
  <div class="picHolder pic2">
    <img src="images/23.jpg" alt="short meeting">
  </div>
</section>
