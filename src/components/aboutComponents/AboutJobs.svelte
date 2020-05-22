<script type="text/javascript">
  export let job;
  export let jobDescription;
</script>

<style type="text/css">
  .isJob {
    /*height: 100%;
    width: 100%;*/
    color: #fff;
    background-color: #ff1d1d;
    padding: 25px;
    position: relative;
  }

  h2 {
    /*font-size: 1.2rem;*/
    font-weight: 700;
    margin: 0;
  }

  h3 {
    position: absolute;
    bottom: 0;
    right: 0;
    font-weight: 700;
    padding-right: 25px;
    padding-bottom: 25px;
  }

  p {
    margin: 0;
  }

  .isArrow {
    display: inline-block;
    font-size: 1.5rem;
    color: #fff;
    background-color: #ff1d1d;
    position: absolute;
    bottom: 0;
    left: 0;
    padding: 0 7px;
    margin-left: 25px;
    margin-bottom: 25px;
    border-radius: 50%;
  }

  .isArrow:hover {
    color: #ff1d1d;
    background-color: #fff;
    margin-bottom: 25px;
  }
</style>

<div class="isJob">
  <h2>{job}</h2>
  <p>{jobDescription}</p>
  <h3>apply now!</h3>
  <p class="isArrow">&#10132;</p>
</div>
