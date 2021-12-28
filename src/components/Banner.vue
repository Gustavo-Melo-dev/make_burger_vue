<template>
  <div id="banner">
    <h1>Monte o seu hambúrguer</h1>
  </div>
</template>

<script>
export default {
    name: "Banner",
}
</script>

<style scoped>
    #banner {
        background-image: url("/img/burger.jpg");
        background-position: 0 -200px;
        background-size: cover;
        height: 600px;
        display: flex;
        align-items: center;
        justify-content: flex-start;
        border-bottom: 4px solid yellow;
    }

    h1 {
        color: yellow;
        text-align: center;
        padding: 20px 40px;
    }
</style>