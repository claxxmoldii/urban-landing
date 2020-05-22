<script type="text/javascript">
  import { fly } from 'svelte/transition';

  export let proj;
  export let visible;
  export let description;
  export let location;
  export let duration;
  export let pic;
</script>

<style type="text/css">
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
    background-color: hsla(0, 100%, 56%, 0.9);/*site color*/
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

  .isInfo .isRotated {
    width: 175px;
    transition-property: bottom left;
    transform:  rotate(-90deg);
    position: absolute;
    right: -50px;
    bottom: 90px;
  }

  .isInfo .isDate {
    font-weight: 700;
  }
</style>

<div class="isProject bgImgFx"
  on:mouseenter={() => {visible = true;}}
  on:mouseleave={() => {visible = false;}}
  style="background-image: url({pic});">
  {#if visible}
    <div  class="isInfo"
          in:fly="{{x: -450, duration: 300}}"
          out:fly="{{x: -450, duration: 300}}">
      <h2>{proj}</h2>
      <h4>{description}</h4>
      <div class="isRotated">
        <p class="isLocation">{location}</p>
        <p class="isDate">{duration}</p>
      </div>
    </div>
  {/if}
</div>
