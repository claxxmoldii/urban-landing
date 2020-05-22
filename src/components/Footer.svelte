<script>
</script>

<style>
  footer {
    color: #888;
    font-size: .8rem;
  }

  p {
    margin: 0;
  }

  .lnr {
    /*display: inline-block;*/
    /*font-size: 20px;*/
  }

  .divider {
    /*height: 10px;*/
    border-top: solid 1px #888;
    margin: 0 20px;
    /*background-color: lightcyan;*/
  }

  .contacts {
    /*background-color: beige;*/
    padding: 10px 0;
    padding-left: 50px;
  }

  .contacts p,
  .contacts i {
    line-height: 2rem;
  }

  .contacts span,
  .contacts i {
    padding-right: 20px;
  }

  .lnr {
    font-size: 1rem;
  }

  .tel {
    padding-right: 10px;
  }

  .email {
    padding-left: 10px;
  }

  .tel:hover, .email:hover {
    color: #ff1d1d;/*site colo*/
    text-decoration: underline;
    cursor: pointer;
  }

  .social:hover {
    color: #ff1d1d;/*site colo*/
    cursor: pointer;
  }
</style>

<svelte:head>
  <link rel="stylesheet" href="https://cdn.linearicons.com/free/1.0.0/icon-font.min.css">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.13.0/css/all.min.css">
</svelte:head>

<footer>
  <div class="divider"></div>
  <div class="contacts">
    <p><span class="lnr lnr-map-marker"></span>
      Rue du Mail - Maliestraat 50 | 1050 Brussels - Belgium
    </p>
    <p><span class="lnr lnr-bubble"></span>
      <span class="tel">+32 (0)2 502 73 28</span> | <span class="email">mail@urbanplatform.com</span>
    </p>
    <i class="social fab fa-instagram"></i>
    <i class="social fab fa-facebook-f"></i>
    <i class="social fab fa-linkedin-in"></i>
    <p>© 2020 Urban Platform | Mentions légales | Site and Identity by HICSELES</p>
  </div>
</footer>
