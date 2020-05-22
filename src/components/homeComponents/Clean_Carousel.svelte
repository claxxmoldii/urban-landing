<script type="text/javascript">
  import { onMount } from 'svelte';
  import { fade } from 'svelte/transition';

  let fadeOut = false;
  let fadeIn = false;
  let flash = false;
  let isOut;
  let isIn;

  let slideTop;
  let slideUnder;
  let slideFisrt;
  let slideLast;

  let divis;

  let placeholder = 'imagesGallery/1.jpg';

  const slides = [
    'imagesGallery/1.jpg',
    'imagesGallery/2.jpg',
    'imagesGallery/3.jpg',
    'imagesGallery/4.jpg',
    'imagesGallery/5.jpg',
    'imagesGallery/6.jpg'
  ];

  const setDelay = () => {
    setTimeout(() => {
      slide6.classList.remove('isOut');
    }, 5000)
  }

  const fader = (slide) => {
    setTimeout(() => {
      slide.classList.add('fadeOut');
      // slide.classList.add('isOut');
    }, 5000);
  }

  const darthFader = (slideOut, slideIn) => {
    setTimeout(() => {
      slideIn.classList.remove('isOut');
      slideOut.classList.add('fadeOut');
      slideOut.classList.add('isOut');
    }, 5000);
  }

  function onSuccess () {
  console.log('Success!')
}

function onError () {
  console.log('💩')
}

const promise = new Promise((resolve, reject) => {
  setTimeout(() => {
    resolve()
  }, 2000)
})

promise.then(onSuccess)
promise.catch(onError)

function getPromise () {
  return new Promise((resolve) => {
    setTimeout(resolve, 2000)
  })
}

function logA () {
  console.log('A')
}

function logB () {
  console.log('B')
}

function logCAndThrow () {
  console.log('C')

  throw new Error()
}

function catchError () {
  console.log('Error!')
}

getPromise()
  .then(logA) // A
  .then(logB) // B
  .then(logCAndThrow) // C
  .catch(catchError) // Error!

$("#btn").on("click", () => {
  const user = await getUser('tylermcginnis') // SyntaxError: await is a reserved word
  const weather = await getWeather(user.location) // SyntaxError: await is a reserved word

  updateUI({
    user,
    weather,
  })
})

  onMount(async () => {
    const slides = document.querySelectorAll('.bgImgFx');
    const len = slides.length;//7
    const numOfSlides = len - 1;//6

    const slide1 = slides.item(0);
    const slide2 = slides.item(1);
    const slide3 = slides.item(2);
    const slide4 = slides.item(3);
    const slide5 = slides.item(4);
    const slide6 = slides.item(5);

    slide6.classList.remove('isOut');
    // fader(slide6);
  });

  //loop through all divis... okay
  //timer seems okay... okay

  //flash function...
  //xmas tree loop function...
  //xmas tree flash loop...
</script>

<style type="text/css">
  .carousel {
    display: grid;
    grid-template-columns: [window] 100%;
  }

  .bgImgFx {
    background: no-repeat center center;
    background-size: cover;
    height: 100vh;
    width: 100%;
    /*grid-area: window;*/
  }

  .flash {
    animation: fade-out 2s 5s ease-in-out alternate 1;
  }

  .fadeIn {
    animation: fade-out 2s ease-in;
  }

  .fadeOut {
    animation: fade-out 2s 5s ease-out;
  }

  .isOut {
    opacity: 0;
  }

  @keyframes fade-out {
    0% {
      opacity: 1;
    }
    100% {
      opacity: 0;
    }
  }

  @keyframes fade-in {
    0% {
      opacity: 0;
    }
    100% {
      opacity: 1;
    }
  }
</style>


<div id ="carousel" class="carousel">
  {#each slides as slide, index}
    {#if index}
      <div  class="bgImgFx isOut"
            class:fadeIn
            class:fadeOut
            class:flash
            style="background-image: url({slide});">
      </div>
    {/if}
  {/each}
</div>
