<script type="text/javascript">
  import AboutTeamSlider from './AboutTeamSlider.svelte';
</script>

<style type="text/css">
  section {
    height: auto;
    display: grid;
    padding-bottom: 50px;
    grid-template-rows: [carousel] auto [teamPic] auto [teamMems] auto;
  }

  .isCarousel {
    grid-row: carousel;
    max-width: calc(100vw - 150px);
    overflow-x: hidden;
    margin-bottom: 50px;
  }

  .teamPic {
    grid-row: teamPic;
    max-width: calc(100vw - 150px);
    padding: 0 50px;
    margin-bottom: 25px;
    height: auto;
  }

  .teamPic img {
    width: 100%;
    height: auto;
  }

  .teamMems {
    grid-row: teamMems;
    position: relative;
    margin: 0 auto;
  }

  .teamMems h4 {
    display: inline-block;
    position: absolute;
    top: 97px;
    left: -80px;
    transition-property: bottom right;
    transform: rotate(-90deg);
    font-family: 'Open Sans', 'Raleway', sans-serif;
    font-weight: 700;
  }

  .teamMems ul {
    width: 550px;
  }

  .teamMems li {
    display: inline-block;
    font-size: 0.9rem;
  }

  .teamMems li:after{
    content: '|';
    color: #ff1d1d;
    padding-left: 10px;
    padding-right: 8px;
  }

  .teamMems .isFounder {
    font-weight: 700;
  }
</style>

<section>
  <div class="isCarousel">
    <AboutTeamSlider />
  </div>

  <div class="teamPic">
    <img src="imagesAbout/team-2.jpg" alt="team photo
    ">
  </div>

  <div class="teamMems">
    <h4 class="siteColor">they worked with us</h4>
    <ul>
      <li class="isFounder">Olivier Perier - Founding Partner</li>
      <li class="isFounder">Eveline Vyncke - Partner</li>
      <li>Najiw Zemmouri</li>
      <li>Franck Casaubon</li>
      <li>Stéphanie Perrini</li>

      <li>Laura Martinez</li>
      <li>Alexandre Lhussa</li>
      <li>Camille Vande Putte</li>
      <li>Céline Sauvage</li>
      <li>Félicien Umbreit</li>

      <li>Iago Pineda</li>
      <li>Tina Van Meenen</li>
      <li>Nuria Ribas</li>
      <li>Carine Borghans</li>
      <li>Maria Cantizano</li>

      <li>Kaat Volckaert</li>
      <li>Christophe Van Raemdonck</li>
      <li>Delia Aniorte Soria</li>
      <li>Stijn Thomas</li>
      <li>Emmanuelle Poels</li>

      <li>Yvan Breithof</li>
      <li>Karel Deckers</li>
      <li>Bassam El-Okeily</li>
      <li>Marwen Feriani</li>
      <li>Gérald Ledent</li>

      <li>Marie Henrard</li>
      <li>Constance Lambert</li>
      <li>Francisco Gaslo</li>
      <li>Louisiane Desbrosses</li>
      <li>Nathalie Touwaide</li>

      <li>Sarah Vanhamme</li>
      <li>Dien Wiersma</li>
      <li>Riccardo Carati</li>
      <li>Eleonora Campanella</li>
      <li>Christopher Gramer</li>

      <li>Mathieu Bourdon</li>
      <li>Bastien de Harven</li>
      <li>Quentin Lemal</li>
      <li>Nathanaëlle Poels</li>
      <li>Luc Pecourt</li>

      <li>Diana Palade</li>
      <li>Sophie Courouble</li>
      <li>Mateusz Chodorowski</li>
      <li>Béatrix Woringer</li>
      <li>Sanne Berghmans</li>

      <li>Géraldine de Neuville</li>
      <li>Thibaut Rome</li>
      <li>Adrien Morelli</li>
      <li>Laurence Lambert</li>
      <li>Sandra Princzkelova</li>

      <li>Thomas Van Bouwel</li>
      <li>Diego Sanchez</li>
      <li>Martin Janssens</li>
      <li>Nele De Raedt</li>
      <li>Christel Van Poeyer</li>

      <li>Charles-Diego Leonet</li>
      <li>Olivier Roegiest</li>
    </ul>
  </div>
</section>
