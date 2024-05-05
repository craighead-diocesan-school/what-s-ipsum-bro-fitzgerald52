<script>
  import Snav from '../../lib/Snav.svelte'
</script>

<Snav />
<main>
  <div class="subheading">
    <div class="cherries">
      <img class="actual" src="/cherry.png" alt="cherry" />
      <img class="shadow" src="/whitecherry.png" alt="cherry" />
    </div>
    <h2>Yum Cupcake Ipsum</h2>
    <div class="cherries">
      <img class="actual" src="/cherry.png" alt="cherry " />
      <img class="shadow" src="/whitecherry.png" alt="cherry" />
    </div>
  </div>
  <div class="text">
    <p>Halvah liquorice apple pie jelly beans chupa chups candy icing tiramisu. Tart jelly jujubes gingerbread croissant biscuit. Chupa chups tart cheesecake lemon drops dragée chocolate bar dessert. Ice cream ice cream sugar plum jujubes dragée topping tiramisu croissant chocolate.</p>

    <p>Jujubes tiramisu gingerbread cake donut chocolate bar tart marzipan pastry. Gingerbread jelly tootsie roll muffin bear claw muffin. Jelly-o fruitcake chocolate bar chupa chups chocolate sesame snaps candy. Sweet roll carrot cake cake jelly candy jujubes gummi bears jelly-o. Oat cake wafer chocolate bar sweet roll macaroon soufflé powder sugar plum tart.</p>
  </div>
</main>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Pacifico&display=swap');
  .text {
    background-color: rgb(165, 106, 42);
    height: 350px;
    padding: 25px;
  }

  p {
    justify-content: center;
    background-color: rgb(255, 246, 236, 0.5);
    padding: 50px;
    text-align: center;
  }
  .subheading {
    display: flex;
    align-items: center;
    justify-content: space-around;
    background: url(/icing.jpg);
    padding: 30px;
    background-position: cover;
    color: aliceblue;
    font-family: 'Pacifico', cursive;
    font-weight: 400;
    font-size: xx-large;
    text-align: center;
  }
  .cherries {
    position: relative;
  }
  .shadow {
    position: absolute;
    top: 0;
    left: 0;
    transform: scale(1.15);
    z-index: 0.1;
  }
  .actual {
    position: relative;
    z-index: 100000;
  }
  main {
    margin-left: 300px;
    margin-right: 300px;
  }
  @media screen and (max-width: 1000px) {
    main {
      margin-left: 10px;
      margin-right: 10px;
    }
  }
</style>
