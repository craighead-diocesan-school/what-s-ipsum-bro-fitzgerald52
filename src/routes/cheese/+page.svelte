<script>
  import Header from '$lib/Header.svelte'
  import Footer from '$lib/Footer.svelte'
</script>

<Header color="yellow" />

<main>
  <h2>Pee-YOO Cheese Ipsum</h2>

  <div class="text">
    <p>Cheesy grin parmesan taleggio. Brie boursin pecorino cheesy feet taleggio hard cheese roquefort when the cheese comes out everybody's happy. St. agur blue cheese port-salut bocconcini cheesecake rubber cheese mozzarella stilton cheese strings. Bocconcini.</p>

    <p>Fromage the big cheese camembert de normandie. Cut the cheese gouda brie the big cheese when the cheese comes out everybody's happy squirty cheese cut the cheese gouda. Boursin cottage cheese cheeseburger camembert de normandie cheese slices goat port-salut danish fontina. Emmental caerphilly cream cheese mozzarella camembert de normandie cheesy feet.</p>
  </div>

  <!-- <div class="boxes"> -->
  <a class="piratehole" href="/pirate">
    <img class="pirateicon" src="/pirate.png" alt="Pirate" />
  </a>
  <a class="homehole" href="/">
    <img class="homeicon" src="/home.png" alt="home page " />
  </a>
  <a class="cupcakehole" href="cupcake">
    <img class="cupcakeicon" src="/cupcake.png" alt="Cupcake" />
  </a>
  <a class="hipsterhole" href="hipster">
    <img class="hipstericon" src="/hipster.png" alt="Hipster" />
  </a>
  <!-- </div> -->
</main>

<Footer />

<style>
  main {
    margin: 5em 10em;
    padding: 3em 3em;
    display: grid;
    grid:
      ' .  z z  . ' auto
      ' .  t t  p ' auto
      ' i  t t  c ' auto
      ' .  h  . . ' auto
      / 1fr 6fr;
  }

  .text {
    font-family: 'Patrick Hand', cursive;
    width: 30%;
    grid-area: t;
  }
  .piratehole {
    grid-area: p;
  }

  .cupcakehole {
    grid-area: c;
  }

  .hipsterhole {
    grid-area: i;
  }

  .homehole {
    grid-area: h;
  }

  main {
    background-color: #ffff00;
  }
  h2 {
    text-align: center;
    font-family: 'Patrick Hand', cursive;
    grid-area: z;
  }

  .piratehole:hover .pirateicon {
    transform: scale(1.1);
    transition: 0.25s;
  }
  .piratehole {
    width: 125px;
    height: 125px;
    border-radius: 50%;
    padding: 25px;
    background: rgb(211, 211, 36);
    /* box-shadow: 15px 15px rgb(156, 152, 88); change to be inside */
    transform: scale(1);
    transition: 0.25s;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .homehole:hover .homeicon {
    transform: scale(1.1);
    transition: 0.25s;
  }
  .homehole {
    width: 125px;
    height: 125px;
    border-radius: 50%;
    padding: 25px;
    background: rgb(211, 211, 36);
    /* box-shadow: 15px 15px rgb(156, 152, 88); change to be inside */
    transform: scale(1);
    transition: 0.25s;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .cupcakehole:hover .cupcakeicon {
    transform: scale(1.1);
    transition: 0.25s;
  }
  .cupcakehole {
    width: 125px;
    height: 125px;
    border-radius: 50%;
    padding: 25px;
    background: rgb(211, 211, 36);
    /* box-shadow: 15px 15px rgb(156, 152, 88); change to be inside */
    transform: scale(1);
    transition: 0.25s;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .hipsterhole:hover .hipstericon {
    transform: scale(1.1);
    transition: 0.25s;
  }
  .hipsterhole {
    width: 125px;
    height: 125px;
    border-radius: 50%;
    padding: 25px;
    background: rgb(211, 211, 36);
    /* box-shadow: 15px 15px rgb(156, 152, 88); change to be inside */
    transform: scale(1);
    transition: 0.25s;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  img {
    transform: scale(0);
    transition: 0.25s;
  }
  img:hover {
    transform: scale(1.5);
    transition: 0.25s;
  }

  @media screen and (max-width: 1000px) {
    main {
      width: 100vw;
      display: inline-block;
      margin: 0px;
    }
    h2 {
      width: 100vw;
    }
  }
</style>
