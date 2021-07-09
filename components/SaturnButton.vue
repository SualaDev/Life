<template>
  <div class="container">
    <div class="btncontainer">
      <button class="btn-1">
        Placeholder
      </button>
      <button class="btn-2">
        Placeholder
      </button>
      <button class="btn-3">
        Placeholder
      </button>
      <button class="btn-4">
        Placeholder
      </button>
      <button class="btn-5">
        Placeholder
      </button>
      <button class="btn-6">
        Placeholder
      </button>
    </div>
    <div class="btncontainer">
      <button class="btn-1b">
        <p>Placeholder</p>
        <img src="~assets/image/white.svg" alt="" :class="WhiteIcon">
      </button>
      <button class="btn-2b">
        <p>Placeholder</p>
        <img src="~assets/image/white.svg" alt="">
      </button>
      <button class="btn-3b">
        <p>Placeholder</p>
        <img src="~assets/image/white.svg" alt="">
      </button>
      <button class="btn-4b">
        <p>Placeholder</p>
        <img src="~assets/image/orange.svg" alt="" :class="OrangeIcon">
      </button>
      <button class="btn-5b">
        <p>Placeholder</p>
        <img src="~assets/image/darkgrey.svg" alt="" :class="DarkGreyIcon">
      </button>
      <button class="btn-6b">
        <p>Placeholder</p>
        <img src="~assets/image/lightgrey.svg" alt="" :class="LightGreyIcon">
      </button>
    </div>
  </div>
</template>

<script>
</script>

<style>
.btncontainer{
  display:flex;
  flex-wrap: wrap;
  width:50%;
  margin-bottom: 50px;
}
button{
margin-right: 2%;
margin-bottom: 2%;
width:188px;
height:50px;
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

.btn-1b{
  border-radius: 20px;
  background-color:#F87023;
  padding:0 24px ;
  color:white;
  border:none;
  display:flex;
  justify-content: space-between;
  align-items: center;
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
}
</style>
