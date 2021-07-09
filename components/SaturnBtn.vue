<template>
  <div>
    <button :class="btnstyle" class="btn">
      Placeholder
    </button>
  </div>
</template>

<script>
export default {
  props: {
    btnstyle: String
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
