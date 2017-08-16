<template>
  <div id="app">
    <header>
      <div class="wrapper">
        <router-link to="/"><img src="./assets/images/logo.png" alt="" class="logo"></router-link>
        <div class="text">
          <h2 class="text--title">Picture Perfect</h2>
          <p class="text--info">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequatur, nam, necessitatibus quo pariatur rem libero. Ipsa, voluptates, harum, iusto magnam excepturi explicabo ex aperiam deleniti repudiandae amet aspernatur omnis. Eaque.</p>
        </div>
      </div>
    </header>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css?family=Open+Sans');

body {
  margin: 0;
  font-family: "Open Sans";
}

.wrapper {
  width: 80%;
  max-width: 1180px;
  margin: 0 auto;
}

#app {
  header {
    width: 100%;
    height: 100vh;
    background-image: url('./assets/images/background.png');
    background-size: cover;
    background-repeat: no-repeat;
    color: #fff;

    .logo {
      margin-top: 55px;
    }

    .text {
      width: 440px;
      margin-top: 20%;

      &--title {
        font-size: 60px;
      }

      &--info {
        font-size: 13px;
        line-height: 1.2;
      }
    }
  }
}
</style>
