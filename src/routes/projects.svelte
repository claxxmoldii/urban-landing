<script type="text/javascript">
  import { fly } from 'svelte/transition';
  // import NavProjects from '../components/navComponents/NavProjects.svelte';
  import SelectedProjects from '../components/projectsComponents/SelectedProjects.svelte';

  const rabelaise = {
          proj: 'rabelaise',
          visible: false,
          description: 'renovation of school site and facilities in the heart of Ixelles',
          location: 'brussels - belgium',
          duration: '2019 - on going',
          pic: 'imagesProjects/80.jpg'
        };

  const marchandises = {
          proj: 'marchandises',
          visible: false,
          description: 'a block with a range of allocations',
          location: 'brussels - belgium',
          duration: '2018 - on going',
          pic: 'imagesProjects/70.jpg'
        };

  const waterloo = {
          proj: 'waterloo',
          visible: false,
          description: 'construction of social dwellings and facilities',
          location: 'brussels - belgium',
          duration: '2017 - on going',
          pic: 'imagesProjects/66.jpg'
        };

  const alexianen = {
          proj: 'alexianen',
          visible: false,
          description: 'conversion of a school site into a mixed-use project and public park',
          location: 'tienen - belgium',
          duration: '2016 - on going',
          pic: 'imagesProjects/56.jpg'
        };

  const tenbosch = {
          proj: 'tenbosch',
          visible: false,
          description: 'construction of dwellings',
          location: 'brussels - belgium',
          duration: '2011 - 2019',
          pic: 'imagesProjects/35.jpg'
        };

  const houille = {
          proj: 'houille',
          visible: false,
          description: 'dwellings in a dense context',
          location: 'brussels - belgium',
          duration: '2014 - 2019',
          pic: 'imagesProjects/58.jpg'
        };

  const immac2 = {
          proj: 'immac2',
          visible: false,
          description: 'conversion of a heritage site into a mixed-use project',
          location: 'tienen - belgium',
          duration: '2014 - 2019',
          pic: 'imagesProjects/55.jpg'
        };

  const harmonie = {
          proj: 'harmonie',
          visible: false,
          description: 'day centre and dwellings for the elderly',
          location: 'brussels - belgium',
          duration: '2012 - on going',
          pic: 'imagesProjects/50.jpg'
        };

  const lochten = {
          proj: 'lochten',
          visible: false,
          description: 'susteainable micro-neighbourhood',
          location: 'brussels - belgium',
          duration: '2012 - 2019',
          pic: 'imagesProjects/49.jpg'
        };

  const lutgardisHousing = {
          proj: 'lutgardisHousing',
          visible: false,
          description: 'restrcuturing of a block with facilities and dwellings',
          location: 'brussels - belgium',
          duration: '2011 - 2019',
          pic: 'imagesProjects/79.jpg'
        };

  const lutgardisSchool = {
          proj: 'lutgardisSchool',
          visible: false,
          description: 'restructuring of a school site',
          location: 'brussels - belgium',
          duration: '2011 - 2017',
          pic: 'imagesProjects/47.jpg'
        };

  const pegasus = {
          proj: 'pegasus',
          visible: false,
          description: 'extension of a school campus',
          location: 'oostende - belgium',
          duration: '2011 - 2015',
          pic: 'imagesProjects/46.jpg'
        };

  const castel = {
          proj: 'castel',
          visible: false,
          description: 'fractal house',
          location: 'brussels - belgium',
          duration: '2010 - 2013',
          pic: 'imagesProjects/41.jpg'
        };

  const fancy = {
          proj: 'fancy',
          visible: false,
          description: 'rethinking industrial buildings',
          location: 'seneffe - belgium',
          duration: '2008 - 2009',
          pic: 'imagesProjects/33.jpg'
        };

  const lens = {
          proj: 'fancy',
          visible: false,
          description: 'dwellings behins a folding façade',
          location: 'brussels - belgium',
          duration: '2005 - 2012',
          pic: 'imagesProjects/26.jpg'
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
<!--   <nav>
    <NavProjects />
  </nav>
 -->  <main>
    <SelectedProjects {...rabelaise}/>
    <SelectedProjects {...marchandises}/>
    <SelectedProjects {...waterloo}/>
    <SelectedProjects {...alexianen}/>
    <SelectedProjects {...tenbosch}/>
    <SelectedProjects {...houille}/>
    <SelectedProjects {...immac2}/>
    <SelectedProjects {...harmonie}/>
    <SelectedProjects {...lochten}/>
    <SelectedProjects {...lutgardisHousing}/>
    <SelectedProjects {...lutgardisSchool}/>
    <SelectedProjects {...pegasus}/>
    <SelectedProjects {...castel}/>
    <SelectedProjects {...fancy}/>
    <SelectedProjects {...lens}/>
  </main>
  <footer></footer>
</section>
