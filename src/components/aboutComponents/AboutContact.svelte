<script type="text/javascript">
  import { onMount } from 'svelte';

  let brussels = 'imagesAbout/brussels.png'//map placeholder bgimage

  let container;
  let map;
  let zoom = 16;
  let maliestraat = {lat: 50.822152, lng: 4.360047};
  let center = maliestraat;
  let current = 'maliestraat';

  const maliestraatMarker = new google.maps.Marker({
    position: maliestraat,
    map: map
  });

  onMount(async () => {
    map = new google.maps.Map(container, {
      zoom,
      center
    });
    maliestraatMarker.setMap(map);
  });

</script>

<style type="text/css">
  section {
    padding: 0 50px;
    display: grid;
    grid-template-columns: [addresses] 1fr [map] 1fr;
  }

  p {
    font-size: .9rem;
  }

  span {
    font-weight: 200;
    padding-top: 5px;
    color: hsla(0, 100%, 56%, 0.8);
  }

  .isAddresses {
    grid-column: addresses;
  }

  .address {
    display: grid;
    grid-template-columns: [marker] 60px [address] auto;
    padding-bottom: 25px;
  }

  .address *,
  .tel * {
    margin: 0;
  }

  .address span {
    grid-column: marker;
    font-size: 1.5rem;
  }

  .address p {
    grid-column: address;
  }

  .tel {
    display: grid;
    grid-template-columns: [balloon] 60px [tel] auto;
    /*padding-bottom: 25px; */
  }

  .tel span {
    grid-column: balloon;
    font-size: 1.5rem;
  }

  .tel div {
    grid-column: tel;
  }

  .isMap {
    grid-column: map;
    width: 100%;
    height: 400px;
  }

  .isTheMap {
    /*width: 100%;*/
    /*height: 100%;*/
    z-index: 0;
    overflow-x: hidden;
    filter: grayscale(99%); /*grayscale fx*/
  }

  .bgImgFx {
    background: no-repeat center center;
    background-size: cover;
    overflow: hidden;
    /*height: 100%;
    width: auto;*/
  }
</style>

<section>
  <div class="isAddresses">
    <div class="address">
      <span class="lnr lnr-map-marker"></span>
      <p>Rue du Mail - Maliestraat 50<br/>
          1050 Brussels - Belgium
      </p>
    </div>

    <div class="tel">
      <span class="lnr lnr-bubble"></span>
      <div>
        <p class="telephone">Tel: +32 (0)2 502 73 28</p>
        <p class="email">mail@urbanplatform.com</p>
      </div>
    </div>
  </div>

  <div  class="isMap isTheMap bgImgFx"
        bind:this={container}
        style="background-image: url({brussels});">
  </div>
</section>
