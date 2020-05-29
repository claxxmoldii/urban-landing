<script type="text/javascript">
  export let pic;
  export let name;
  export let title;
  export let superPower;
  export let email;
</script>

<style type="text/css">
  .owl-item {
    width: 70px;
    margin: 0;
  }

  .owl-item:hover .isInfo {
    visibility: visible;
  }

  .owl-item:hover img {
    border-top: solid .8px #ff1d1d;
    border-bottom: solid .8px #ff1d1d;
  }

  .isInfo {
    visibility: hidden;
    padding-top: 20px;
  }

  img {
    width: 100%;
    height: auto;
    border-top: solid .8px #fff;
    border-bottom: solid .8px #fff;
  }

  h4 {
    color: #ff1d1d;
    font-size: .9rem;
    font-weight: 700;
  }

  h5:nth-of-type(2n) {
    color: #ff1d1d;
  }

  a {
    text-decoration: none;
  }

  a:hover {
    text-decoration: underline;
  }
</style>

<div class="owl-item">
  <img src="{pic}" alt="{name}">
  <div class="isInfo">
    <h4>{name}</h4>
    <h5>{title}</h5>
    <h5>{superPower}</h5>
    <h5><a href="mailto:{email}">{email}</a></h5>
  </div>
</div>

<!-- <div class="owl-carousel owl-theme owl-loaded isRelative">
  <div class="owl-stage-outer">
    <div class="owl-stage">
      <div class="owl-item">
        <img src="imagesAbout/4.jpg" alt="larissa walschot">
        <div class="isInfo">
          <h4>larissa walschot</h4>
          <h5>architect</h5>
          <h5>sensibly whole-hearted</h5>
          <h5><a href="mailto:lwa@urbanplatform.com">lwa@urbanplatform.com</a></h5>
        </div>
      </div>
      <div class="owl-item">
        <img src="imagesAbout/5.jpg" alt="clarisse huet">
        <div class="isInfo">
          <h4>clarisse huet</h4>
          <h5>senior architect</h5>
          <h5>joyously well informed</h5>
          <h5><a href="mailto:chu@urbanplatform.com">chu@urbanplatform.com</a></h5>
        </div>
      </div>
      <div class="owl-item">
        <img src="imagesAbout/6.jpg" alt="beatriz perez martin">
        <div class="isInfo">
          <h4>beatriz perez martin</h4>
          <h5>senior ir. architect &amp; urban deisgner</h5>
          <h5>comfortably adventurous</h5>
          <h5><a href="mailto:bpe@urbanplatform.com">bpe@urbanplatform.com</h5>
        </div>
      </div>
      <div class="owl-item">
        <img src="imagesAbout/8.jpg" alt="benoît menu">
        <div class="isInfo">
          <h4>benoît menu</h4>
          <h5>architect</h5>
          <h5>efficient dreamer</h5>
          <h5><a href="mailto:bme@urbanplatform.com">bme@urbanplatform.com</a></h5>
        </div>
      </div>
      <div class="owl-item">
        <img src="imagesAbout/10.jpg" alt="albine delbaere">
        <div class="isInfo">
          <h4>albine delbaere</h4>
          <h5>communication &amp; interior design</h5>
          <h5>rebelliously benevolent</h5>
          <h5><a href="mailto:ade@urbanplatform.com">ade@urbanplatform.com</a></h5>
        </div>
      </div>
      <div class="owl-item">
        <img src="imagesAbout/11.jpg" alt="rosalie lefebvre">
        <div class="isInfo">
          <h4>rosalie lefebvre</h4>
          <h5>junior architect</h5>
          <h5>discretely curious</h5>
          <h5><a href="mailto:rle@urbanplatform.com">rle@urbanplatform.com</a></h5>
        </div>
      </div>
      <div class="owl-item">
        <img src="imagesAbout/12.jpg" alt="marie audag">
        <div class="isInfo">
          <h4>marie audag</h4>
          <h5>senior architect</h5>
          <h5>sensitively determined</h5>
          <h5><a href="mailto:mau@urbanplatform.com">mau@urbanplatform.com</a></h5>
        </div>
      </div>
      <div class="owl-item">
        <img src="imagesAbout/13.jpg" alt="naiara iparragirre gonzalez">
        <div class="isInfo">
          <h4>naiara iparragirre gonzalez</h4>
          <h5>senior ir. architect</h5>
          <h5>precisely inspired</h5>
          <h5><a href="mailto:ni@urbanplatform.com">ni@urbanplatform.com</a></h5>
        </div>
      </div>
      <div class="owl-item">
        <img src="imagesAbout/14.jpg" alt="michiel dehandschutter">
        <div class="isInfo">
          <h4>michiel dehandschutter</h4>
          <h5>senior ir. architect</h5>
          <h5>moving steadily</h5>
          <h5><a href="mailto:mde@urbanplatform.com">mde@urbanplatform.com</a></h5>
        </div>
      </div>
      <div class="owl-item">
        <img src="imagesAbout/16.jpg" alt="apolline vranken">
        <div class="isInfo">
          <h4>apolline vranken</h4>
          <h5>junior architect</h5>
          <h5>flexibly efficient</h5>
          <h5><a href="mailto:avr@urbanplatform.com">avr@urbanplatform.com</a></h5>
        </div>
      </div>
      <div class="owl-item">
        <img src="imagesAbout/17.jpg" alt="julia sprott">
        <div class="isInfo">
          <h4>julia sprott</h4>
          <h5>junior architect</h5>
          <h5>gently straighforward</h5>
          <h5><a href="mailto:jsp@urbanplatform.com">jsp@urbanplatform.com</a></h5>
        </div>
      </div>
      <div class="owl-item">
        <img src="imagesAbout/18.jpg" alt="michael elias">
        <div class="isInfo">
          <h4>michael elias</h4>
          <h5>senior architect</h5>
          <h5>crazily wise</h5>
          <h5><a href="mailto:jsp@urbanplatform.com">mel@urbanplatform.com</a></h5>
        </div>
      </div>
      <div class="owl-item">
        <img src="imagesAbout/19.jpg" alt="véronique tavernier">
        <div class="isInfo">
          <h4>véronique tavernier</h4>
          <h5>architect</h5>
          <h5>energetically focused</h5>
          <h5><a href="mailto:jsp@urbanplatform.com">vta@urbanplatform.com</a></h5>
        </div>
      </div>
      <div class="owl-item">
        <img src="imagesAbout/20.jpg" alt="axelle hamers">
        <div class="isInfo">
          <h4>axelle hamers</h4>
          <h5>junior architect</h5>
          <h5>carefully dynamic</h5>
          <h5><a href="mailto:aha@urbanplatform.com">aha@urbanplatform.com</a></h5>
        </div>
      </div>
      <div class="owl-item">
        <img src="imagesAbout/23.jpg" alt="aitor ugartemendia">
        <div class="isInfo">
          <h4>aitor ugartemendia</h4>
          <h5>architect</h5>
          <h5>nonchalantly committed</h5>
          <h5><a href="mailto:aug@urbanplatform.com">aug@urbanplatform.com</a></h5>
        </div>
      </div>
      <div class="owl-item">
        <img src="imagesAbout/24.jpg" alt="amèlie gressier">
        <div class="isInfo">
          <h4>amèlie gressier</h4>
          <h5>senior architect</h5>
          <h5>pragmatic daydreamer</h5>
          <h5><a href="mailto:agr@urbanplatform.com">agr@urbanplatform.com</a></h5>
        </div>
      </div>
      <div class="owl-item">
        <img src="imagesAbout/25.jpg" alt="sylvain monteiro">
        <div class="isInfo">
          <h4>sylvain monteiro</h4>
          <h5>senior interior architect</h5>
          <h5>practical idealist</h5>
          <h5><a href="mailto:smo@urbanplatform.com">smo@urbanplatform.com</a></h5>
        </div>
      </div>
      <div class="owl-item">
        <img src="imagesAbout/26.jpg" alt="bittor arrillaga">
        <div class="isInfo">
          <h4>bittor arrillaga</h4>
          <h5>architect</h5>
          <h5>rigorously adaptable</h5>
          <h5><a href="mailto:bar@urbanplatform.com">bar@urbanplatform.com</a></h5>
        </div>
      </div>
      <div class="owl-item">
        <img src="imagesAbout/27.jpg" alt="clément panier des touches">
        <div class="isInfo">
          <h4>clément panier des touches</h4>
          <h5>junior architect</h5>
          <h5>creatively perceptive</h5>
          <h5><a href="mailto:cpa@urbanplatform.com">cpa@urbanplatform.com</a></h5>
        </div>
      </div>
      <div class="owl-item">
        <img src="imagesAbout/29.jpg" alt="camille lerquet">
        <div class="isInfo">
          <h4>camille lerquet</h4>
          <h5>junior architect</h5>
          <h5>softly resolute</h5>
          <h5><a href="mailto:cle@urbanplatform.com">cle@urbanplatform.com</a></h5>
        </div>
      </div>
    </div>
  </div>
  <div class="owl-nav naviBox">
      <span class="owl-prev arrow-left">&#10132;</span>
      <span class="owl-next arrow-right">&#10132;</span>
  </div>
</div>
 -->
