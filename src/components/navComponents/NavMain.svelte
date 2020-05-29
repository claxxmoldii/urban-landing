<script>
  export let segment;

  // let current = segment;
</script>

<style>
  section {
    /*max-width: 150px;*/
    /*background-color: beige;*/
    height: 100%;
    /*border-right: solid .5px #dede;*/
  }

  header {
    color: #ff1d1d;/*site colo*/
    padding-bottom: 50px;
  }

  nav {
    /*border-bottom: 1px solid rgba(255,62,0,0.1);*/
    font-weight: 300;
    padding-left: 30px;
  }

  a {
    text-decoration: none;
  }

  .isTitle {
    display: grid;
    grid-template-columns: 100%;
    grid-template-rows: 250px, auto;
    grid-template-areas:
      "mainTitle"
      "subTitle";
  }

  .mainTitle {
    grid-area: mainTitle;
  }

  .mainTitle a {
    font-size: 3rem;
    font-weight: 500;
    writing-mode: vertical-rl;
    transform: rotate(180deg);
    text-align: left;
    line-height: 3rem;
    font-family: 'Open Sans', sans-serif;
    font-weight: 700;
    padding-right: 20px;
    padding-bottom: 30px;
  }

  .subTitle {
    grid-area: subTitle;
    /*border-top: solid 1px #ff1d1d;
    border-bottom: solid 1px #ff1d1d;*/
    padding-left: 30px;
    /*text-align: center;*/

  }

  .subTitle div {
    /*background-color: brown;*/
    border-top: solid 1px #ff1d1d;
    border-bottom: solid 1px #ff1d1d;
    display: inline-block;
  }

  .subTitle div a {
    /*justify-content: left;*/
    text-align: left;
  }

  nav a {
    display: block;
    padding-bottom: 1.5rem;
  }

  .isLink:hover {
    color: darkgray;
    font-weight: inherit;
    cursor: pointer;
  }

  .isdaBlog {
    font-weight: 500;
    color: #ff1d1d;/*site colo*/
  }

  [aria-current] {
    font-weight: 600;
  }
</style>

<section>
  <!-- <header class:selected='{segment === undefined}' href='.'> -->
  <header class="isTitle">
    <div class="mainTitle ">

      <a aria-current='{segment === undefined ? "page" : undefined}'
        href='.'>urban <br/>landing</a>
    </div>
    <div class="subTitle">
      <div>
      <a aria-current='{segment === undefined ? "page" : undefined}'
        href='.'>architecture <br/>urbanism</a>
      </div>
    </div>
  </header>
  <nav>
    <a  class="isLink"
        aria-current='{segment === undefined ? "page" : undefined}'
        href='.'>
        home
    </a>
    <a  class="isLink"
        aria-current='{segment === "projects" ? "page" : undefined}'
        href='projects'>
        projects
    </a>
    <a  class="isLink"
        aria-current='{segment === "practice" ? "page" : undefined}'
        href='practice'>
        practice
    </a>
    <a  class="isLink"
        aria-current='{segment === "about" ? "page" : undefined}'
        href='about'>
        about
    </a>
<!--     <a  class="isLink"
        aria-current='{segment === "success" ? "page" : undefined}'
        href='success'>
        sapper
    </a> -->

    <!-- for the blog link, we're using rel=prefetch so that Sapper prefetches
         the blog data when we hover over the link or tap it on a touchscreen -->
    <a  class="isdaBlog"
        rel=prefetch
        aria-current='{segment === "blog" ? "page" : undefined}'
        href='blog'>
        what's up
    </a>
    <!-- <a class="isdaBlog" rel=prefetch class:selected='{segment === "blog"}' href='blog'>
      what's up
    </a> -->
  </nav>
</section>
