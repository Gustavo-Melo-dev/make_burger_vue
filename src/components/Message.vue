<template>
  <div class="message-container">
    <span>{{ message }}</span>
  </div>
</template>

<script>
export default {
    name: "Message",
    props: {
        message: String
    }
}
</script>

<style>
    .message-container {
        background-color: rgb(175, 245, 175);
        border: 2px solid;
        border-radius: 5px;
        padding: 10px;
        max-width: 400px;
        margin: 30px auto;
    }
</style>