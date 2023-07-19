<template>
  <div class="header">
    <div class="container">
      <router-link :to="{name: 'home'}"><img src="" alt="Logo"></router-link>
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
  border-radius: 0 0 15px 15px;
  box-shadow: 3px 1px 3px rgba(0,0,0, .3);
  .container{
    display: flex;
    justify-content: space-between;
    .menu{
      display: flex;
      gap: 1rem;
      cursor: pointer;
      p:hover{
        color: blue;
      }
    }
  }
}
</style>