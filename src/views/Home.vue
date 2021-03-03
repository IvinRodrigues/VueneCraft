<template>
    <main class="home">

      <section class="title-section">
        <img src="https://www.logaster.com/blog/wp-content/uploads/2020/06/image14-3.png">
      </section>

      <section class="buttons-section">
        <button><span>Singleplayer</span></button>
        <button><span>Multiplayer</span></button>
        <button><span>Minecraft Realms</span></button>
      </section>

    </main>
</template>

<script>

export default {
  name: 'Home',
  components: {
  }
}
</script>

<style lang="scss">

  @font-face {

    font-family: minecraft;
    src: url('../assets/fonts/minecraft.ttf');

  }

  .mine-font {

    font-family: minecraft;

  }

  main {

    background: brown;
    height: 100vh;
    width: 100vw;

    .title-section {

      display: flex;
      justify-content: center;
      
      img { width: 900px; }

    }

    .buttons-section {

      display: flex;
      flex-direction: column;
      align-items: center;

      button {

      font-family: minecraft;
      font-size: 1.4rem;
      color: white;
      text-shadow: 4px 4px 0 rgba(0, 0, 0, 0.200);
      width: 594px;
      height: 54px;
      background: gray;
      display: block;
      padding-top: 1rem;
      margin: .5rem 0;
      border: 4px solid black;
      font-weight: 100;
      background-image: url('../assets/images/button-shape.png');
      position: relative;
      transition-duration: .2s;

      span { 
      
        display: block;
        position: relative;
        top: -8px;
        
      }

      &:hover { 
        
        border-color: white;
        transform: scale(1.02);
        
      }

      }

    }

}

</style>