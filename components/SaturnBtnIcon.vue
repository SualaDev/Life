<template>
  <div>
    <button class="iconBtn">
      <p>Placeholder</p>
      <img :src="image">
    </button>
  </div>
</template>

<script>
export default {
  props: {
    image: String
  }
}
</script>

<style>
.iconBtn{
  background-color: rebeccapurple;
}
</style>
