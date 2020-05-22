<style type="text/css">
  section {
    height: auto;
    padding: 0 50px;
    padding-bottom: 50px;
    display: grid;
    grid-template-columns: [pic] 1fr [partners] 1fr;
  }

  h4 {
    font-weight: 700;
  }

  h5 {
    font-size: 0.9rem;
  }

  address {
    display: inline-block;
  }

  a {
    text-decoration: none;
    font-style: normal;
  }

  a:hover {
    text-decoration: underline solid #ff1d1d;
  }

  p {
    font-size: 0.9rem;
  }

  .pic {
    grid-column: pic;
    width: 400px;
    height: 300px;
    overflow: hidden;
    background-color: beige;
  }

  .pic img {
    width: 100%;
    height: auto;
    margin-top: -50px;
  }

  .arePartners {
    grid-column: partners;
    background-color: light;
  }
</style>

<section>
  <div class="pic">
    <img src="imagesAbout/7.jpg" alt="partners photo">
  </div>

  <div class="arePartners">
    <h4>Cédric Franck</h4>
    <h5><span class="siteColor">Madly enthusiastic</span>  |  <address><a href="cfr@urbanplatform.com">cfr@urbanplatform.com</a></address></h5>
    <p>
      Co-founder of Urban Platform in 2000 with Alicia Reiber and Olivier Périer, he practices as architect since 1994 . As Managing Partner, he is responsible for managing the agency and leads the private projects of our two platforms.
    </p>

    <h4>Alicia Reiber</h4>
    <h5><span class="siteColor">Creatively meticulous</span>  |  <address><a href="are@urbanplatform.com">are@urbanplatform.com</a></address></h5>
    <p>
      Co-founder of Urban Platform in 2000 with Cédric Franck and Olivier Périer, she practices as architect since 1997. As Partner, she leads the design department of the agency.
    </p>

    <h4>Xavier Lostrie</h4>
    <h5><span class="siteColor">Flexibly accurate</span>  |  <address><a href="xlo@urbanplatform.com">xlo@urbanplatform.com</a></address></h5>
    <p>
      Joined Urban Platform in 2012 and became partner in 2016. He practices as architect since 2007. As Partner, he leads the public projects of our two platforms.
    </p>
  </div>
</section>
