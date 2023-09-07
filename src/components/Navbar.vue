<template>
  <div class="header">
    <div class="container">
      <router-link :to="{name: 'home'}"><span>Noleto.</span></router-link>
      <nav class="menu">
        <router-link :to="{name: 'home'}"><p>Menu 1</p></router-link>
        <router-link :to="{name: 'home'}"><p>Menu 2</p></router-link>
        <router-link :to="{name: 'home'}"><p>Menu 3</p></router-link>
      </nav>
    </div>
  </div>
</template>
<script>
export default{
  name: 'Navbar',
}
</script>
<style lang="scss" scoped>
.header{
  width: 100%;
  padding: 1.5rem 0;
  border-bottom: 1px solid #999;
  box-shadow: 3px 1px 3px rgba(0,0,0, .3);
  .container{
    display: flex;
    justify-content: space-between;
    span{
      font-size: 22px;
    }
    .menu{
      display: flex;
      gap: 1rem;
      cursor: pointer;
      font-size: 16px;
      p:hover{
        color: var(--color2);
      }
    }
  }
}
</style>