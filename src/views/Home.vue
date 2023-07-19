<template>
  <section>
    <div class="container">
      <div class="introduction">
        <h3>Oi, eu sou Ramon</h3>
        <div class="technologies">
          <h2>VUE</h2>
          <img src="./../../public/vuejs-icon.svg" alt="Vue.js">
        </div>
        <h2>Developer<span>.</span></h2>
      </div>
  </div>
  </section>
</template>

<script>
export default{
  name: 'Home',
  data(){
    return{
      Tecnologies:[
        {
          icon:'./../../public/vuejs-icon.svg',
          name:'Vue.JS',
        },
      ],
    }
  }
}
</script>

<style lang="scss" scoped>
.container{
  padding: 1rem;
  .introduction{
    width: max-content;
    padding: 1rem;
    letter-spacing: -1px;
    .technologies{
      align-items: baseline;
      display: flex;
      gap: 0.5rem;
      img{
        width: 20px;
        clip-path: circle();
        padding: 0.5rem;
        background-color: #98f0c8;
      }
    }
    h2{
      font-size: 40px;
      margin-bottom: -15px;
      span{
        color: blue;
      }
    }
  }
}
</style>