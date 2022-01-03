<template>
  <div id="footer">
    <p>{{ footer }} &copy; 2021 <br> 
    Instagram: <a href="https://www.instagram.com/guumelo/" target="_blank">Gustavo Melo</a> <br>
    Linkedin: <a href="https://www.linkedin.com/in/gustavo-melo-a3ba73199/" target="_blank">Gustavo Melo</a></p>
  </div>
</template>

<script>
export default {
  name: "Footer",
  props: ['footer'],
}
</script>

<style scoped>
  #footer {
    height: 100px;
    display: flex;
    justify-content: center;
    align-items: center;
    background: #222;
    border-top: 3px solid yellow;
    color: yellow;
    bottom: 0;
    position: fixed;
    width: 100%;
  }

  a {
    color: yellow;
  }
</style>