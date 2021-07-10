<template>
  <div class="container">
    <div class="btncontainer">
      <SaturnBtn btnstyle="btn-1 " w-icon="del-icon" o-icon="del-icon" d-icon="del-icon" l-icon="del-icon" />
      <SaturnBtn btnstyle="btn-2" w-icon="del-icon" o-icon="del-icon" d-icon="del-icon" l-icon="del-icon" />
      <SaturnBtn btnstyle="btn-3" w-icon="del-icon" o-icon="del-icon" d-icon="del-icon" l-icon="del-icon" />
      <SaturnBtn btnstyle="btn-4" w-icon="del-icon" o-icon="del-icon" d-icon="del-icon" l-icon="del-icon" />
      <SaturnBtn btnstyle="btn-5" w-icon="del-icon" o-icon="del-icon" d-icon="del-icon" l-icon="del-icon" />
      <SaturnBtn btnstyle="btn-6" w-icon="del-icon" o-icon="del-icon" d-icon="del-icon" l-icon="del-icon" />
      <SaturnBtn btnstyle="btn-1b" o-icon="del-icon" d-icon="del-icon" l-icon="del-icon" />
      <SaturnBtn btnstyle="btn-2b" o-icon="del-icon" d-icon="del-icon" l-icon="del-icon" />
      <SaturnBtn btnstyle="btn-3b" o-icon="del-icon" d-icon="del-icon" l-icon="del-icon" />
      <SaturnBtn btnstyle="btn-4b" w-icon="del-icon" d-icon="del-icon" l-icon="del-icon" />
      <SaturnBtn btnstyle="btn-5b" w-icon="del-icon" o-icon="del-icon" l-icon="del-icon" />
      <SaturnBtn btnstyle="btn-6b" w-icon="del-icon" o-icon="del-icon" d-icon="del-icon" />
    </div>
    <!-- <div class="btncontainer">
      <SaturnBtnIcon image="~/assets/image/orange.svg" />
    </div> -->
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
}
.btn-1{
  border-radius: 20px;
  background-color:#F87023;
  padding:17px 54px 18px 54px;
  color:white;
  border:none;
  margin-top: 20px;
  margin-left: 20px;
}
.btn-2{
  border-radius: 20px;
  background-color:#5D6A73;
  padding:17px 54px 18px 54px;
  color:white;
  border:none;
  margin-top: 20px;
  margin-left: 20px;
}

.btn-3{
  border-radius: 20px;
  background-color:#BBBBBB;
  padding:17px 54px 18px 54px;
  color:white;
  border:none;
  margin-top: 20px;
  margin-left: 20px;
}

.btn-4{
  border-radius: 20px;
  background-color:white;
  padding:17px 54px 18px 54px;
  color:#F87023;
  border:1px solid #F87023;
  margin-top: 20px;
  margin-left: 20px;
}

.btn-5{
  border-radius: 20px;
  background-color:white;
  padding:17px 54px 18px 54px;
  color:#5D6A73;
  border:1px solid #5D6A73;
  margin-top: 20px;
  margin-left: 20px;
}

.btn-6{
  border-radius: 20px;
  background-color:#bbbbbb85;
  padding:17px 54px 18px 54px;
  color:#BBBBBB;
  border:1px solid #BBBBBB ;
  margin-top: 20px;
  margin-left: 20px;
}

.btn-1b{
  border-radius: 20px;
  background-color:#F87023;
  padding:0 24px ;
  color:white;
  border:none;
  display:flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 20px;
  margin-left: 20px;
}

.btn-2b{
  border-radius: 20px;
  background-color:#5D6A73;
  padding:0 24px;
  color:white;
  border:none;
  display:flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 20px;
  margin-left: 20px;
}

.btn-3b{
  border-radius: 20px;
  background-color:#BBBBBB;
  padding:0 24px;
  color:white;
  border:none;
  display:flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 20px;
  margin-left: 20px;
}

.btn-4b{
  border-radius: 20px;
  background-color:white;
  padding:0 24px;
  color:#F87023;
  border:1px solid #F87023;
  display:flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 20px;
  margin-left: 20px;
}

.btn-5b{
  border-radius: 20px;
  background-color:white;
  padding:0 24px;
  color:#5D6A73;
  border:1px solid #5D6A73;
  display:flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 20px;
  margin-left: 20px;
}

.btn-6b{
  border-radius: 20px;
  background-color:transparent;
  padding:0 24px;
  color:#BBBBBB;
  border:1px solid #BBBBBB ;
  display:flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 20px;
  margin-left: 20px;
}

.del-icon{
  display: none;
}
</style>
