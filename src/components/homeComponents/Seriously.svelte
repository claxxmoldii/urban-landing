<script type="text/javascript">
  // let isBanner = 'images/seriously.svg';
  let isBanner = 'images/seriously-02.svg';
  let isArrow = 'images/arrow.svg';
</script>

<style type="text/css">
  div {
    position: fixed;
    top: 0;
    right: 0;
    bottom: 0;
    left: 150px;
  }

  header {
    min-height: 100vh;
    max-width: 100%;
    z-index: 100;
    display: flex;
    flex-direction: column;
    justify-content: flex-end;
    /*background-color: beige;*/
  }

  .isBanner{
    width: 400px;
    height: auto;
    align-self: center;
    padding-bottom: 100px;
  }

  .isArrow {
    height: auto;
  }
</style>

<div>
  <header>
    <img class="isBanner"src={isBanner} alt="seriosuly creative.">
    <img class="isArrow" src={isArrow}>
  </header>
</div>
