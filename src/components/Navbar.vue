<template>
  <div id="nav">
    <div class="image">
        <router-link to="/"><img :src="logo" :alt="description"></router-link>
    </div>
    <router-link to="/">Home</router-link>
    <span>|</span>
    <router-link to="/requests">Pedidos</router-link>
  </div>
</template>

<script>
export default {
  name: "Navbar",
  props: ['logo', 'description']
}
</script>

<style scoped>
  #nav {
    background: #222;
    border-bottom: 3px solid yellow;
    padding: 15px 50px;
    display: flex;
    justify-content: flex-end;
    align-items: center;
  }

  .image {
    margin: auto;
    margin-left: 0px;
  }

  img {
    width: 40px;
    height: 40px;
  }

  #nav a {
    color: yellow;
    text-decoration: none;
    margin: 10px;
    transition: 0.5s;
  }

  #nav a:hover {
    color: rgb(102, 102, 1);
  }

  span {
    color: white;
  }
</style>