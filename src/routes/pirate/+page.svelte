<script>
  import Snav from '../../lib/Snav.svelte'
</script>

<Snav />
<main>
  <div class="subheading">
    <img src="/skull.png" alt="skull face " />
    <h2>Yar Pirate Ipsum</h2>
    <img src="/skull.png" alt="skull face " />
  </div>

  <div class="container">
    <div class="background">
      <p>Maroon square-rigged rope's end spirits fathom tackle bilge rat careen cackle fruit splice the main brace. Arr to go on account bilge six pounders smartly yo-ho-ho yawl tack boatswain maroon. Barque hogshead coffer Buccaneer loot fire ship Shiver me timbers Blimey salmagundi reef.</p>

      <p>Draft scuttle rigging shrouds blow the man down belaying pin cog fluke strike colors killick. Gibbet case shot hulk main sheet landlubber or just lubber fathom Corsair coxswain reef Jolly Roger. Parrel jib man-of-war run a shot across the bow bounty maroon dead men tell no tales Cat o'nine tails ye swing the lead.</p>
    </div>
  </div>
</main>

<style>
  h2 {
    font-family: hyper-scrypt;
    color: #d9edff;
    font-size: xxx-large;
  }
  .subheading {
    display: flex;
    align-items: center;
    justify-content: space-around;
    background: url(/flag.png);
    height: 150px;
  }
  .background {
    background: url(/ship.gif);
    background-repeat: no-repeat;
    display: flex;
    align-items: center;
    background-position: left;
    height: 500px;
    padding: 20px;
    transition: 5s;
  }
  .background:hover {
    background-position: right;
    transition: 5s;
  }
  main {
    height: 500px;
  }
  .container {
    background: url(/sea.gif);
    height: 500px;
    display: flex;
    align-items: center;
    background-position: center;
  }
  p {
    font-family: basteleur;
    background-color: rgba(255, 255, 255, 0.5);
    margin: 20px;
    padding: 20px;
    transition: 2s;
  }
  p:hover {
    transition: 2s;
    background-color: #880808;
    transform: scale(1.1);
  }

  @media screen and (max-width: 1000px) {
    .background {
      flex-direction: column;
    }
    .container {
      width: 110vw;
    }
    h2 {
      font-family: hyper-scrypt;
      color: #d9edff;
      font-size: medium;
    }
    .subheading {
      width: 110vw;
    }
  }
</style>
