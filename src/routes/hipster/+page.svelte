<script>
  import Snav from '../../lib/Snav.svelte'
</script>

<Snav />
<main>
  <h2>You Probably Haven't Heard of Hipster Ipsum</h2>

  <div class="top">
    <p>Fingerstache tofu pickled vibecession kitsch lyft blackbird spyplane vegan craft beer keytar banh mi thundercats. Hashtag heirloom vape scenester paleo hexagon. Blackbird spyplane pok pok DIY heirloom scenester food truck kale chips pabst, bitters raw denim artisan waistcoat seitan freegan.</p>
  </div>
  <div class="bottom">
    <p>Put a bird on it vibecession fashion axe YOLO asymmetrical. VHS photo booth listicle fam truffaut subway tile yr cred chicharrones semiotics biodiesel green juice microdosing whatever. Truffaut praxis PBR and B tattooed street art. Prism jean shorts pickled vegan. Vegan praxis cronut kitsch pop-up. Letterpress street art mlkshk marxism.</p>
  </div>
  <a class="tree" href="/treestump">
    <img class="trunk" src="/treestump.png" alt="tree trunk" />
  </a>
  <a href="/plane">
    <img class="plane" src="/plane.gif" alt="white plane" />
  </a>
</main>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Rubik+Bubbles&display=swap');
  h2 {
    color: aliceblue;
    grid-area: h;
    font-family: Rubik bubbles;
    font-size: xx-large;
    text-align: center;
  }
  main {
    background-color: rgb(59, 143, 238);

    display: grid;
    grid:
      ' h h p   ' auto
      ' t t .   ' auto
      ' r b .  ' auto;
  }
  .top {
    grid-area: t;
    background-color: rgb(43, 173, 20, 0.5);
    padding: 30px;
    border-radius: 20%;
    font-family: monospace;
    width: 1000px;
  }
  .bottom {
    grid-area: b;
    background-color: rgb(43, 173, 20, 0.5);
    padding: 30px;
    border-radius: 20%;
    font-family: monospace;
    width: 800px;
    height: 200px;
  }

  .tree {
    grid-area: r;
    width: 200px;
  }
  .trunk {
    width: 200px;
  }
  .plane {
    grid-area: p;
    width: 200px;
  }
</style>
