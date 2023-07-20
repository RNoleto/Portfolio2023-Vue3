<template>
  <section>
    <div class="container">
      <div class="introduction">
        <h3>Oi, eu sou Ramon</h3>
        <div class="social">
          <h2>VUE</h2>
          <div class="social-icons" v-for="(social,index) in Socials" :key="index">
            <img :src="social.icon" :alt="social.name">
          </div>
        </div>
        <h2>Developer<span>.</span></h2>
        <p>
          Tenho 35 anos sou desenvolvedor frontend com 3 anos de experiencia trabalhando como autonomo. Gosto de aprender novas tecnologias e criar ferramentas que possam ajudar várias pessoas.
        </p>
      </div>
      <div class="tecnologies">
        <div class="card" v-for="(tecnologie, index) in Tecnologies" :key="index">
          <img :src="tecnologie.icon" :alt="tecnologie.name">
        </div>
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
        {
          icon: './../../public/html-5-svgrepo-com.svg',
          name: 'Html5',
        },
        {
          icon: './../../public/css-3-svgrepo-com.svg',
          name: 'CSS',
        },
        {
          icon: './../../public/sass-svgrepo-com.svg',
          name: 'Sass',
        },
        {
          icon: './../../public/javascript-svgrepo-com.svg',
          name: 'JavaScript',
        },
      ],
      Socials: [
        {
          icon: './../public/github-142-svgrepo-com.svg',
          name: 'Github',
          link: '',
        },
        {
          icon: './../public/linkedin-round-svgrepo-com.svg',
          name: 'Linkedin',
          link: '',
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.container{
  padding: 1rem;
  color: var(--color5);
  .introduction{
    width: auto;
    padding: 1rem;
    letter-spacing: -1px;

    border: 1px solid var(--color4);
    border-radius: 15px;
    background-color: var(--color2);
    h2{
      font-size: 40px;
      margin-bottom: -15px;
      span{
        color: var(--color3);
      }
    }
    p{
      margin-top: 0.5rem;
      line-height: 18px;
    }
    .social{
      display: flex;
      gap: 0.5rem;
      align-items: baseline;

      margin: -15px 0;
      &-icons{
        img{
          width: 30px;
        }
      }
    }
  }
  .tecnologies{
    display: flex;
    justify-content: center;
    gap: 0.2rem;
    img{
      width: 45px;
    }
  }
}
</style>