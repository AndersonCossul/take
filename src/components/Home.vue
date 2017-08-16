<template>
  <main class="wrapper">
    <div class="presentation">
      <div class="presentation--box">
        <h2 class="presentation--box__title">{{ primaryContent.left.title }}</h2>
        <p class="presentation--box__text" v-html="primaryContent.left.text"></p>
      </div>
      <img src=".././assets/images/phone.png" class="presentation--phone">
      <div class="presentation--box">
        <p class="presentation--box__text" v-html="primaryContent.right.text"></p>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: 'home',
  data () {
    return {
      primaryContent: {
        left: {
          title: 'Start something cool',
          text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ipsum illo dolor nostrum quibusdam similique facilis totam quis voluptatem iure, amet cum ullam nesciunt molestiae porro necessitatibus modi itaque. Asperiores, amet.<br/><br/>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quibusdam ducimus nam, debitis natus modi eum obcaecati quae veniam soluta porro assumenda, eveniet quis deserunt minus doloremque iste veritatis eaque. Neque?<br/><br/>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laborum molestiae fugiat quos laboriosam suscipit pariatur odio iure inventore tenetur, ipsam beatae excepturi. Expedita harum amet asperiores, quod, magni quae veniam.'
        },
        right: {
          text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sint quae, itaque ipsam! Quod ipsum ex unde rem, velit facilis tempora expedita pariatur, nihil maxime. Eveniet aut voluptatum quae ut consequatur!<br/><br/>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aperiam tempora impedit rerum libero odio, sit, minima veniam commodi facere, sapiente iusto quisquam ea id deleniti totam molestiae nisi eveniet in!'
        }
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
  main {
    .presentation {
      &--box {
        margin-top: 120px;
        width: 39%;
        margin-right: 10%;
        display: inline-block;
        vertical-align: bottom;

        &__title {
          font-size: 35px;
          color: #222626;
          font-weight: 100;
        }

        &__text {
          font-size: 14px;
          color: #959595;
        }
      }

      &--phone {
        position: absolute;
        top: -350px;
        right: 0;
        width: 600px;
      }
    }
  }
</style>
