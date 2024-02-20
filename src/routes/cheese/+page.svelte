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

  <div class="boxes">
    <a class="circle" href="/pirate">
      <img src="pirate.png" alt="Pirate" />
    </a>
    <a class="circle" href="/">
      <img src="home.png" alt="home page " />
    </a>
    <a class="circle" href="cupcake">
      <img src="cupcake.png" alt="Cupcake" />
    </a>
    <a class="circle" href="hipster">
      <img src="hipster.png" alt="Hipster" />
    </a>
  </div>
</main>

<Footer />

<style>
  main {
    background-color: #ffff00;
  }
  h2 {
    text-align: center;
    font-family: 'Patrick Hand', cursive;
  }
  .boxes {
    display: flex;
    flex-wrap: wrap;
    gap: 25px;
    justify-content: space-between;
    width: 400px;
  }
  .circle:hover {
    transform: scale(1.1);
    transition: 0.25s;
  }
  .circle {
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
    transform: scale(0.1);
    transition: 0.25s;
  }
  img:hover {
    transform: scale(1.5);
    transition: 0.25s;
  }
  .text {
    font-family: 'Patrick Hand', cursive;
    width: 30%;
  }
</style>
