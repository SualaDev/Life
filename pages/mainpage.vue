<template>
  <div class="container">
    <div class="btncontainer">
      <SaturnBtn btnstyle="btn-1" />
      <SaturnBtn btnstyle="btn-2" />
      <SaturnBtn btnstyle="btn-3" />
      <SaturnBtn btnstyle="btn-4" />
      <SaturnBtn btnstyle="btn-5" />
      <SaturnBtn btnstyle="btn-6" />
    </div>
    <div class="btncontainer">
      <SaturnBtnIcon image="~/assets/image/orange.svg" />
    </div>
  </div>
</template>

<script>
export default {
}
</script>

<style>
.btncontainer{
  display:flex;
  flex-wrap: wrap;
  width:50%;
  margin-bottom: 50px;
}
.btn-1{
  border-radius: 20px;
  background-color:#F87023;
  padding:17px 54px 18px 54px;
  color:white;
  border:none;
}
.btn-2{
  border-radius: 20px;
  background-color:#5D6A73;
  padding:17px 54px 18px 54px;
  color:white;
  border:none;
}

.btn-3{
  border-radius: 20px;
  background-color:#BBBBBB;
  padding:17px 54px 18px 54px;
  color:white;
  border:none;
}

.btn-4{
  border-radius: 20px;
  background-color:white;
  padding:17px 54px 18px 54px;
  color:#F87023;
  border:1px solid #F87023;
}

.btn-5{
  border-radius: 20px;
  background-color:white;
  padding:17px 54px 18px 54px;
  color:#5D6A73;
  border:1px solid #5D6A73;
}

.btn-6{
  border-radius: 20px;
  background-color:#bbbbbb85;
  padding:17px 54px 18px 54px;
  color:#BBBBBB;
  border:1px solid #BBBBBB ;
}
</style>
