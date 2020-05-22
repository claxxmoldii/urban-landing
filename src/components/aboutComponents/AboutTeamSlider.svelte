<script type="text/javascript">
  import { onMount } from 'svelte';
  import AboutOwlItem from './AboutOwlItem.svelte';

  const shione = {
    pic: 'imagesAbout/300.jpg',
    name: 'shione cooper',
    title: 'super architect',
    superPower: 'huge tits!',
    email: 'DDD@urbanplatform.com'
  }

  const larissa = {
    pic: 'imagesAbout/4.jpg',
    name: 'larissa walschot',
    title: 'architect',
    superPower: 'sensibly whole-hearted',
    email: 'lwa@urbanplatform.com'
  }

  const clarisse = {
    pic: 'imagesAbout/5.jpg',
    name: 'clarisse huet',
    title: 'senior architect',
    superPower: 'joyously well informed',
    email: 'chu@urbanplatform.com'
  }

  const beatriz = {
    pic: 'imagesAbout/6.jpg',
    name: 'beatriz perez martin',
    title: 'senior ir. architect &amp; urban deisgner',
    superPower: 'comfortably adventurous',
    email: 'bpe@urbanplatform.com'
  }

  const benoît = {
    pic: 'imagesAbout/8.jpg',
    name: 'benoît menu',
    title: 'architect',
    superPower: 'efficient dreamer',
    email: 'bme@urbanplatform.com'
  }

  const albine = {
    pic: 'imagesAbout/10.jpg',
    name: 'albine delbaere',
    title: 'communication &amp; interior design',
    superPower: 'rebelliously benevolent',
    email: 'ade@urbanplatform.com'
  }



  const rosalie = {
    pic: 'imagesAbout/11.jpg',
    name: 'rosalie lefebvre',
    title: 'junior architect',
    superPower: 'discretely curious',
    email: 'rle@urbanplatform.com'
  }

  const marie = {
    pic: 'imagesAbout/12.jpg',
    name: 'marie audag',
    title: 'senior architect',
    superPower: 'sensitively determined',
    email: 'mau@urbanplatform.com'
  }

  const naiara = {
    pic: 'imagesAbout/13.jpg',
    name: 'naiara iparragirre gonzalez',
    title: 'senior ir. architect',
    superPower: 'precisely inspired',
    email: 'ni@urbanplatform.com'
  }

  const michiel = {
    pic: 'imagesAbout/14.jpg',
    name: 'michiel dehandschutter',
    title: 'senior ir. architect',
    superPower: 'moving steadily',
    email: 'mde@urbanplatform.com'
  }

  const apolline = {
    pic: 'imagesAbout/16.jpg',
    name: 'apolline vranken',
    title: 'junior architect',
    superPower: 'flexibly efficient',
    email: 'avr@urbanplatform.com'
  }

  const julia = {
    pic: 'imagesAbout/17.jpg',
    name: 'julia sprott',
    title: 'junior architect',
    superPower: 'gently straighforward',
    email: 'jsp@urbanplatform.com'
  }

  const michael = {
    pic: 'imagesAbout/18.jpg',
    name: 'michael elias',
    title: 'senior architect',
    superPower: 'crazily wise',
    email: 'mel@urbanplatform.com'
  }

  const véronique = {
    pic: 'imagesAbout/19.jpg',
    name: 'véronique tavernier',
    title: 'architect',
    superPower: 'energetically focused',
    email: 'vta@urbanplatform.com'
  }

  const axelle = {
    pic: 'imagesAbout/20.jpg',
    name: 'axelle hamers',
    title: 'junior architect',
    superPower: 'carefully dynamic',
    email: 'aha@urbanplatform.com'
  }

  const aitor = {
    pic: 'imagesAbout/23.jpg',
    name: 'aitor ugartemendia',
    title: 'architect',
    superPower: 'nonchalantly committed',
    email: 'aug@urbanplatform.com'
  }

  const amèlie = {
    pic: 'imagesAbout/24.jpg',
    name: 'amèlie gressier',
    title: 'senior architect',
    superPower: 'pragmatic daydreamer',
    email: 'agr@urbanplatform.com'
  }

  const sylvain = {
    pic: 'imagesAbout/25.jpg',
    name: 'sylvain monteiro',
    title: 'senior interior architect',
    superPower: 'practical idealist',
    email: 'smo@urbanplatform.com'
  }

  const bittor = {
    pic: 'imagesAbout/26.jpg',
    name: 'bittor arrillaga',
    title: 'architect',
    superPower: 'rigorously adaptable',
    email: 'bar@urbanplatform.com'
  }

  const clément = {
    pic: 'imagesAbout/27.jpg',
    name: 'clément panier des touches',
    title: 'junior architect',
    superPower: 'creatively perceptive',
    email: 'cpa@urbanplatform.com'
  }

  const camille = {
    pic: 'imagesAbout/29.jpg',
    name: 'camille lerquet',
    title: 'junior architect',
    superPower: 'softly resolute',
    email: 'cle@urbanplatform.com'
  }

  let jackQuery;

  onMount(async () => {
    jackQuery = jQuery.noConflict();

    jackQuery(document).ready(function(){
      jackQuery('.owl-carousel').owlCarousel({
        loop: true,
        autoplay: true,
        autoplayTimeout: 5000,
        margin: 25,
        center: true,
        dots: false,
        // nav: true,
        lazyLoad: true,
        responsive: {
          0:    { items:1 },
          600:  { items:3 },
          1000: { items:6 }
        }
      })
    });

    var owl = jackQuery('.owl-carousel');

    jackQuery('.owl-next').click(function() {
      owl.trigger('next.owl.carousel', [300]);
    })

    jackQuery('.owl-prev').click(function() {
      owl.trigger('prev.owl.carousel', [300]);
    });

  });
</script>

<style type="text/css">
  .owl-carousel {
    max-width: 100%;
    position: relative;
  }

  .isRelative {
    position: relative;
  }

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

  .naviBox {
    width: 90%;
    position: relative;
    /*top: 100px;*/
    /*left: 50px;*/
    /*background-color: lightcyan;*/
    /*display: flex;
    flex-direction: row;
    justify-content: space-between;*/
  }

  span {
    font-size: 1.5rem;
    color: #ff1d1d;
    background-color: #fff;
    border-radius: 50%;
    padding: 0 7px;
  }

  span:hover {
    color: #fff;
    background-color: #ff1d1d;
  }

  .arrow-left {
    transform: rotate(180deg);
    position: absolute;
    top: 35%;
    left: 80px;
  }

  .arrow-right {
    position: absolute;
    top: 35%;
    right: 80px;
  }

  a {
    text-decoration: none;
  }

  a:hover {
    text-decoration: underline;
  }
</style>

<svelte:head>
  <link rel="stylesheet" href="owlcarousel/owl.carousel.min.css">
  <link rel="stylesheet" href="owlcarousel/owl.theme.default.min.css">
</svelte:head>

<div class="owl-carousel owl-theme owl-loaded isRelative">
  <div class="owl-stage-outer">
    <div class="owl-stage">

      <AboutOwlItem {...shione} />

      <AboutOwlItem {...larissa} />
      <AboutOwlItem {...clarisse} />
      <AboutOwlItem {...beatriz} />
      <AboutOwlItem {...benoît} />
      <AboutOwlItem {...albine} />

      <AboutOwlItem {...rosalie} />
      <AboutOwlItem {...marie} />
      <AboutOwlItem {...naiara} />
      <AboutOwlItem {...michiel} />
      <AboutOwlItem {...apolline} />

      <AboutOwlItem {...julia} />
      <AboutOwlItem {...michael} />
      <AboutOwlItem {...véronique} />
      <AboutOwlItem {...axelle} />
      <AboutOwlItem {...aitor} />

      <AboutOwlItem {...amèlie} />
      <AboutOwlItem {...sylvain} />
      <AboutOwlItem {...bittor} />
      <AboutOwlItem {...clément} />
      <AboutOwlItem {...camille} />

    </div>
  </div>
  <span class="owl-prev arrow-left">&#10132;</span>
  <span class="owl-next arrow-right">&#10132;</span>
  <!-- <div class="owl-nav naviBox">
      <span class="owl-prev arrow-left">&#10132;</span>
      <span class="owl-next arrow-right">&#10132;</span>
  </div> -->
</div>
