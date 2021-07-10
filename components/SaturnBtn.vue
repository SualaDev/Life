<template>
  <div>
    <button :class="btnstyle" class="btn">
      <p>Placeholder</p>
      <img src="~assets/image/white.svg" alt="" :class="WIcon">
      <img src="~assets/image/orange.svg" alt="" :class="OIcon">
      <img src="~assets/image/darkgrey.svg" alt="" :class="DIcon">
      <img src="~assets/image/lightgrey.svg" alt="" :class="LIcon">
    </button>
  </div>
</template>

<script>
export default {
  props: {
    btnstyle: String,
    WIcon: String,
    OIcon: String,
    DIcon: String,
    LIcon: String
  }

}
</script>

<style>
button{
margin-right: 2%;
margin-bottom: 2%;
width:188px;
height:50px;
}
</style>
