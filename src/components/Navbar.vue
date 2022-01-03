<template>
  <div id="nav">
    <div class="image">
        <router-link to="/"><img :src="logo" :alt="description"></router-link>
    </div>
    <div class="btn-header">
      <router-link to="/">Home</router-link>
    </div>
      <span>|</span>
      <div class="btn-header">
      <router-link to="/requests">Pedidos</router-link>
    </div>
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
    color: black;
    text-decoration: none;
    margin: 10px;
    transition: 0.5s;
  }

  #nav a:hover {
    color: black;
  }

  span {
    color: yellow;
  }

  .btn-header {
    background: yellow;
    border-radius: 20px;
    margin: 10px;
    padding: 5px;
  }
  .btn-header:hover {
    background-color: white;
  }
</style>