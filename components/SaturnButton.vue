<template>
  <div>
    <div class="btncontainer">
      <button class="btn1">
        Placeholder
      </button>
      <button class="btn2">
        Placeholder
      </button>
      <button class="btn3">
        Placeholder
      </button>
      <button class="btn4">
        Placeholder
      </button>
      <button class="btn5">
        Placeholder
      </button>
      <button class="btn6">
        Placeholder
      </button>
    </div>
    <div class="btncontainer">
      <button class="btn1b">
        <p>Placeholder</p>
        <img src="~assets/image/white.svg" alt="">
      </button>
      <button class="btn2b">
        <p>Placeholder</p>
        <img src="~assets/image/white.svg" alt="">
      </button>
      <button class="btn3b">
        <p>Placeholder</p>
        <img src="~assets/image/white.svg" alt="">
      </button>
      <button class="btn4b">
        <p>Placeholder</p>
        <img src="~assets/image/orange.svg" alt="">
      </button>
      <button class="btn5b">
        <p>Placeholder</p>
        <img src="~assets/image/darkgrey.svg" alt="">
      </button>
      <button class="btn6b">
        <p>Placeholder</p>
        <img src="~assets/image/lightgrey.svg" alt="">
      </button>
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
button{
margin-right: 2%;
margin-bottom: 2%;
width:188px;
height:50px;
}
.btn1{
  border-radius: 20px;
  background-color:#F87023;
  padding:17px 54px 18px 54px;
  color:white;
  border:none;
}

.btn2{
  border-radius: 20px;
  background-color:#5D6A73;
  padding:17px 54px 18px 54px;
  color:white;
  border:none;
}

.btn3{
  border-radius: 20px;
  background-color:#BBBBBB;
  padding:17px 54px 18px 54px;
  color:white;
  border:none;
}

.btn4{
  border-radius: 20px;
  background-color:white;
  padding:17px 54px 18px 54px;
  color:#F87023;
  border:1px solid #F87023;
}

.btn5{
  border-radius: 20px;
  background-color:white;
  padding:17px 54px 18px 54px;
  color:#5D6A73;
  border:1px solid #5D6A73;
}

.btn6{
  border-radius: 20px;
  background-color:#bbbbbb85;
  padding:17px 54px 18px 54px;
  color:#BBBBBB;
  border:1px solid #BBBBBB ;
}

.btn1b{
  border-radius: 20px;
  background-color:#F87023;
  padding:0 24px ;
  color:white;
  border:none;
  display:flex;
  justify-content: space-between;
  align-items: center;
}

.btn2b{
  border-radius: 20px;
  background-color:#5D6A73;
  padding:0 24px;
  color:white;
  border:none;
  display:flex;
  justify-content: space-between;
  align-items: center;
}

.btn3b{
  border-radius: 20px;
  background-color:#BBBBBB;
  padding:0 24px;
  color:white;
  border:none;
  display:flex;
  justify-content: space-between;
  align-items: center;
}

.btn4b{
  border-radius: 20px;
  background-color:white;
  padding:0 24px;
  color:#F87023;
  border:1px solid #F87023;
  display:flex;
  justify-content: space-between;
  align-items: center;
}

.btn5b{
  border-radius: 20px;
  background-color:white;
  padding:0 24px;
  color:#5D6A73;
  border:1px solid #5D6A73;
  display:flex;
  justify-content: space-between;
  align-items: center;
}

.btn6b{
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
