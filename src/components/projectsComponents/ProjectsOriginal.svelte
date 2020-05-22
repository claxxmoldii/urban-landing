<script type="text/javascript">
  import { fly } from 'svelte/transition';
  import NavProjects from '../components/NavProjects.svelte';
  import SelectedProjects from '../components/projectsComponents/SelectedProjects.svelte';

  let rabelaise = {visible: false, img: 'imagesProjects/80.jpg'};
  let marchandises = {visible: false, img: 'imagesProjects/70.jpg'};
  let waterloo = {visible: false, img: 'imagesProjects/66.jpg'};
  let alexianen = {visible: false, img: 'imagesProjects/56.jpg'};
  let tenbosch = {visible: false, img: 'imagesProjects/35.jpg'};
  let houille = {visible: false, img: 'imagesProjects/58.jpg'};
  let immac2 = {visible: false, img: 'imagesProjects/55.jpg'};
  let harmonie = {visible: false, img: 'imagesProjects/50.jpg'};
  let lochten = {visible: false, img: 'imagesProjects/49.jpg'};
  let lutgardisHousing = {visible: false, img: 'imagesProjects/79.jpg'};
  let lutgardisSchool = {visible: false, img: 'imagesProjects/47.jpg'};
  let pegasus = {visible: false, img: 'imagesProjects/46.jpg'};
  let castel = {visible: false, img: 'imagesProjects/41.jpg'};
  let fancy = {visible: false, img: 'imagesProjects/33.jpg'};
  let lens = {visible: false, img: 'imagesProjects/26.jpg'};

  const coffeeShop = {
        proj: 'coffeeShop',
        visible: false,
        description: 'really nice here... desu!',
        location: 'brussels - belgium',
        duration: '2019 - on going',
        pic: 'imagesProjects/coffeeShop.jpg'
  };
</script>

<style type="text/css">
  nav {
    position: fixed;
    /*background-color: beige;*/
    background-color: #fff;
    z-index: 100;
  }

  main {
    min-height: 100vh;
    max-width: 100%;
    position: relative;
    padding: 0 50px;
    padding-top: 150px;
    /*background-color: lightcyan;*/
  }

  main {
    display: grid;
    /*margin: 0 auto;*/
    grid-template-columns: 1fr 1fr;
    grid-auto-rows: minmax(315px, auto);
    column-gap: 20px;
    row-gap: 20px;
  }

  .isProject {
    height: 315px;
    width: 100%;
  }

  .bgImgFx {
    background: no-repeat center center;
    background-size: cover;
    overflow: hidden;
    /*height: 100%;
    width: auto;*/
  }

  .isInfo {
    background-color: hsla(0, 100%, 56%, 0.9);
    height: 100%;
    color: white;
    position: relative;
  }

  .isInfo h2 {
    font-weight: 800;
    padding-top: 10px;
    padding-left: 10px;
  }

  .isInfo h4 {
    padding-left: 10px;
    /*font-size: 0.9rem;*/
    font-weight: 300;
    display: inline-block;
    max-width:250px;
    word-wrap:break-word;
  }

  .isInfo p {
    line-height: 1.2rem;
    margin: 0;
    padding: 0;
  }

  .isInfo .rotato {
    transition-property: bottom left;
    transform:  translateX(200px)
                translateY(-60px)
                rotate(-90deg);
  }

  .isInfo .rotato-adjusto {
    transition-property: bottom left;
    transform:  translateX(200px)
                translateY(-40px)
                rotate(-90deg);
  }

  .isInfo .isDate {
    font-weight: 700;
  }

  footer {
    height: 60px;
    width: 100%;
    /*background-color: beige;*/
  }
</style>

<svelte:head>
	<title>Projects</title>
</svelte:head>

<section>
  <nav>
    <NavProjects />
  </nav>
  <main>
    <div class="isProject rabelaise bgImgFx"
      on:mouseenter={() => {rabelaise.visible = true;}}
      on:mouseleave={() => {rabelaise.visible = false;}}
      style="background-image: url({rabelaise.img});">
      {#if rabelaise.visible}
        <div  class="isInfo absPos"
              in:fly="{{x: -450, duration: 300}}"
              out:fly="{{x: -450, duration: 300}}">
          <h2>rabelaise</h2>
          <h4>renovation of school site and facilities in the heart of Ixelles</h4>
          <div class="rotato">
            <p class="isLocation">brussels - belgium</p>
            <p class="isDate">2019 - on going</p>
          </div>
        </div>
      {/if}
    </div>

    <div class="isProject marchandises bgImgFx"
      on:mouseenter={() => {marchandises.visible = true;}}
      on:mouseleave={() => {marchandises.visible = false;}}
      style="background-image: url({marchandises.img});">
      {#if marchandises.visible}
        <div  class="isInfo absPos"
              in:fly="{{x: -450, duration: 300}}"
              out:fly="{{x: -450, duration: 300}}">
          <h2>marchandises</h2>
          <h4>a block with a range of allocations</h4>
          <div class="rotato-adjusto">
            <p class="isLocation">brussels - belgium</p>
            <p class="isDate">2018 - on going</p>
          </div>
        </div>
      {/if}
    </div>

    <div class="isProject waterloo bgImgFx"
      on:mouseenter={() => {waterloo.visible = true;}}
      on:mouseleave={() => {waterloo.visible = false;}}
      style="background-image: url({waterloo.img});">
      {#if waterloo.visible}
        <div  class="isInfo"
              in:fly="{{x: -450, duration: 300}}"
              out:fly="{{x: -450, duration: 300}}">
          <h2>waterloo</h2>
          <h4>construction of social dwellings and facilities</h4>
          <div class="rotato">
            <p class="isLocation">brussels - belgium</p>
            <p class="isDate">2017 - on going</p>
          </div>
        </div>
      {/if}
    </div>

    <div class="isProject alexianen bgImgFx"
      on:mouseenter={() => {alexianen.visible = true;}}
      on:mouseleave={() => {alexianen.visible = false;}}
      style="background-image: url({alexianen.img});">
      {#if alexianen.visible}
        <div  class="isInfo"
              in:fly="{{x: -450, duration: 300}}"
              out:fly="{{x: -450, duration: 300}}">
          <h2>alexianen</h2>
          <h4>conversion of a school site into a mixed-use project and public park</h4>
          <div class="rotato">
            <p class="isLocation">tienen - belgium</p>
            <p class="isDate">2016 - on going</p>
          </div>
        </div>
      {/if}
    </div>

    <div class="isProject tenbosch bgImgFx"
      on:mouseenter={() => {tenbosch.visible = true;}}
      on:mouseleave={() => {tenbosch.visible = false;}}
      style="background-image: url({tenbosch.img});">
      {#if tenbosch.visible}
        <div  class="isInfo"
              in:fly="{{x: -450, duration: 300}}"
              out:fly="{{x: -450, duration: 300}}">
          <h2>tenbosch</h2>
          <h4>construction of dwellings</h4>
          <div class="rotato-adjusto">
            <p class="isLocation">brussels - belgium</p>
            <p class="isDate">2011 - 2019</p>
          </div>
        </div>
      {/if}
    </div>

    <div class="isProject houille bgImgFx"
      on:mouseenter={() => {houille.visible = true;}}
      on:mouseleave={() => {houille.visible = false;}}
      style="background-image: url({houille.img});">
      {#if houille.visible}
        <div  class="isInfo"
              in:fly="{{x: -450, duration: 300}}"
              out:fly="{{x: -450, duration: 300}}">
          <h2>houille</h2>
          <h4>dwellings in a dense context</h4>
          <div class="rotato-adjusto">
            <p class="isLocation">brussels - belgium</p>
            <p class="isDate">2014 - 2019</p>
          </div>
        </div>
      {/if}
    </div>

    <div class="isProject immac2 bgImgFx"
      on:mouseenter={() => {immac2.visible = true;}}
      on:mouseleave={() => {immac2.visible = false;}}
      style="background-image: url({immac2.img});">
      {#if immac2.visible}
        <div  class="isInfo"
              in:fly="{{x: -450, duration: 300}}"
              out:fly="{{x: -450, duration: 300}}">
          <h2>immac2</h2>
          <h4>conversion of a heritage site into a mixed-use project</h4>
          <div class="rotato">
            <p class="isLocation">tienen - belgium</p>
            <p class="isDate">2014 - 2019</p>
          </div>
        </div>
      {/if}
    </div>

    <div class="isProject harmonie bgImgFx"
      on:mouseenter={() => {harmonie.visible = true;}}
      on:mouseleave={() => {harmonie.visible = false;}}
      style="background-image: url({harmonie.img});">
      {#if harmonie.visible}
        <div  class="isInfo"
              in:fly="{{x: -450, duration: 300}}"
              out:fly="{{x: -450, duration: 300}}">
          <h2>harmonie</h2>
          <h4>day centre and dwellings for the elderly</h4>
          <div class="rotato">
            <p class="isLocation">brussels - belgium</p>
            <p class="isDate">2012 - on going</p>
          </div>
        </div>
      {/if}
    </div>

    <div class="isProject lochten bgImgFx"
      on:mouseenter={() => {lochten.visible = true;}}
      on:mouseleave={() => {lochten.visible = false;}}
      style="background-image: url({lochten.img});">
      {#if lochten.visible}
        <div  class="isInfo"
              in:fly="{{x: -450, duration: 300}}"
              out:fly="{{x: -450, duration: 300}}">
          <h2>lochten</h2>
          <h4>susteainable micro-neighbourhood</h4>
          <div class="rotato">
            <p class="isLocation">brussels - belgium</p>
            <p class="isDate">2012 - 2019</p>
          </div>
        </div>
      {/if}
    </div>

    <div class="isProject lutgardisHousing bgImgFx"
      on:mouseenter={() => {lutgardisHousing.visible = true;}}
      on:mouseleave={() => {lutgardisHousing.visible = false;}}
      style="background-image: url({lutgardisHousing.img});">
      {#if lutgardisHousing.visible}
        <div  class="isInfo"
              in:fly="{{x: -450, duration: 300}}"
              out:fly="{{x: -450, duration: 300}}">
          <h2>lutgardis housing</h2>
          <h4>restrcuturing of a block with facilities and dwellings</h4>
          <div class="rotato">
            <p class="isLocation">brussels - belgium</p>
            <p class="isDate">2011 - 2019</p>
          </div>
        </div>
      {/if}
    </div>

    <div class="isProject lutgardisSchool bgImgFx"
      on:mouseenter={() => {lutgardisSchool.visible = true;}}
      on:mouseleave={() => {lutgardisSchool.visible = false;}}
      style="background-image: url({lutgardisSchool.img});">
      {#if lutgardisSchool.visible}
        <div  class="isInfo"
              in:fly="{{x: -450, duration: 300}}"
              out:fly="{{x: -450, duration: 300}}">
          <h2>lutgardis school</h2>
          <h4>restructuring of a school site</h4>
          <div class="rotato-adjusto">
            <p class="isLocation">brussels - belgium</p>
            <p class="isDate">2011 - 2017</p>
          </div>
        </div>
      {/if}
    </div>

    <div class="isProject pegasus bgImgFx"
      on:mouseenter={() => {pegasus.visible = true;}}
      on:mouseleave={() => {pegasus.visible = false;}}
      style="background-image: url({pegasus.img});">
      {#if pegasus.visible}
        <div  class="isInfo"
              in:fly="{{x: -450, duration: 300}}"
              out:fly="{{x: -450, duration: 300}}">
          <h2>pegasus</h2>
          <h4>extension of a school campus</h4>
          <div class="rotato-adjusto">
            <p class="isLocation">oostende - belgium</p>
            <p class="isDate">2011 - 2015</p>
          </div>
        </div>
      {/if}
    </div>

    <div class="isProject castel bgImgFx"
      on:mouseenter={() => {castel.visible = true;}}
      on:mouseleave={() => {castel.visible = false;}}
      style="background-image: url({castel.img});">
      {#if castel.visible}
        <div  class="isInfo"
              in:fly="{{x: -450, duration: 300}}"
              out:fly="{{x: -450, duration: 300}}">
          <h2>castel</h2>
          <h4>fractal house</h4>
          <div class="rotato-adjusto">
            <p class="isLocation">brussels - belgium</p>
            <p class="isDate">2010 - 2013</p>
          </div>
        </div>
      {/if}
    </div>

    <div class="isProject fancy bgImgFx"
      on:mouseenter={() => {fancy.visible = true;}}
      on:mouseleave={() => {fancy.visible = false;}}
      style="background-image: url({fancy.img});">
      {#if fancy.visible}
        <div  class="isInfo"
              in:fly="{{x: -450, duration: 300}}"
              out:fly="{{x: -450, duration: 300}}">
          <h2>fancy</h2>
          <h4>rethinking industrial buildings</h4>
          <div class="rotato-adjusto">
            <p class="isLocation">seneffe - belgium</p>
            <p class="isDate">2008 - 2009</p>
          </div>
        </div>
      {/if}
    </div>

    <div class="isProject lens bgImgFx"
      on:mouseenter={() => {lens.visible = true;}}
      on:mouseleave={() => {lens.visible = false;}}
      style="background-image: url({lens.img});">
      {#if lens.visible}
        <div  class="isInfo"
              in:fly="{{x: -450, duration: 300}}"
              out:fly="{{x: -450, duration: 300}}">
          <h2>lens</h2>
          <h4>dwellings behins a folding façade</h4>
          <div class="rotato-adjusto">
            <p class="isLocation">brussels - belgium</p>
            <p class="isDate">2005 - 2012</p>
          </div>
        </div>
      {/if}
    </div>

    <SelectedProjects {...coffeeShop}/>

  </main>
  <footer></footer>
</section>
