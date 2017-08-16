<template>
  <main class="wrapper">
    <div class="presentation-box">
      <h2 class="presentation-box--title">{{ title }}</h2>
      <p class="presentation-box--text" v-html="text"></p>
    </div>
  </main>
</template>

<script>
export default {
  name: 'home',
  data () {
    return {
      title: 'Start something cool',
      text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ipsum illo dolor nostrum quibusdam similique facilis totam quis voluptatem iure, amet cum ullam nesciunt molestiae porro necessitatibus modi itaque. Asperiores, amet.<br/><br/>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quibusdam ducimus nam, debitis natus modi eum obcaecati quae veniam soluta porro assumenda, eveniet quis deserunt minus doloremque iste veritatis eaque. Neque?<br/><br/>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laborum molestiae fugiat quos laboriosam suscipit pariatur odio iure inventore tenetur, ipsam beatae excepturi. Expedita harum amet asperiores, quod, magni quae veniam.'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
  main {
    .presentation-box {
      margin-top: 120px;
      width: 40%;
      margin-right: 10%;
    }
  }
</style>
