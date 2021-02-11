<template>
  <div class="home">
    <div class="header">
      <h2 class="title">Hi <b>Cristopher!</b></h2>
      <div class="input">
        <input type="text" placeholder="Find what you want...">
        <div class="icon-input">
          <i class='bx bx-search'></i>
        </div>
      </div>
      <div class="combo-header">
        <div class="text">
          <h3>Free Combo</h3>
          <p>Burger + Coca-Cola for new users</p>
        </div>
        <div class="img">
          <img src="https://images.unsplash.com/photo-1583427548973-3dc79cd09fd4?ixid=MXwxMjA3fDB8MHxzZWFyY2h8NTZ8fHBpenphfGVufDB8fDB8&ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="">
        </div>
      </div>
    </div>
    <div class="scroll-menu">
      <div class="scroll-content">
        <div class="avatar" v-for="(item, index) in 10" :key="index">
          <i class='bx bx-cookie bx-sm'></i>
        </div>
      </div>
    </div>
    <h2>Top Products</h2>
    <div class="scroll-menu">
      <div class="scroll-content">
        <div class="top-products" v-for="(item, index) in 10" :key="index" >
        <div class="top-products-img">
        <img src="https://images.unsplash.com/photo-1553183733-81edd1223a95?ixid=MXwxMjA3fDB8MHxzZWFyY2h8NDR8fGhhbWJ1cmdlcnxlbnwwfHwwfA%3D%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="">
        </div>
        <div class="top-products-text">
          <div class="top-products-title">Berry Juice</div>
          <div class="top-products-price">$7.5</div>
        </div>
        <i class='bx bx-plus-medical'></i>
    </div>
      </div>
    </div>
  </div>
</template>

<style>
  .home{
    margin: 20px;
  }

  .scroll-content-top{
    display: flex;
  }

  .top-products{
    position: relative;
    min-width: 150px;
    background-color:rgba(250, 248, 248);
    padding: 10px;
    border-radius: 10px;
  }

  .top-products-title{
    color: rgba(47, 47, 47,);
  }

  .top-products-text{
    margin-top: 10px;
  }

  .top-products-price{
    color:rgba(255, 131, 62);
  }

  .top-products i{
    position: absolute;
    right: 0;
    bottom: 0;
    padding: 10px;
    color: #fff;
    border-radius: 50px;
    background-color:rgba(74, 174, 84);
    margin: 5px;
  }

  .top-products-img img{
    width: 100%;
  }

  h2{
    font-weight: 400;
  }

  .title{
    margin-top: 60px;
    font-weight: 350;
  }

  .scroll-menu{
    margin-top: 10px;
  }

  .scroll-content{
    display: flex;
    overflow-y: auto;
  }

  .scroll-content::-webkit-scrollbar{
    display: hidden;
  }

  .avatar{
    background-color:rgba(250, 250, 248);
    padding: 20px;
    border-radius: 10px;
    margin: 5px;
  }

  .avatar i{
    color: rgba(255, 131, 62);
  }

  .combo-header{
    background-color:rgba(74, 174, 84);
    color: #fff;
    padding: 20px;
    border-radius: 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 20px;
  }

  .text{
    width: 50%;
  }

  .img{
    width: 50%;
  }

  img{
    width: 100%;
    object-fit: cover;
    border-radius: 10px;
  }

  h3{
    font-weight: 400;
  }

  p{
    font-weight: 300;
  }

  .input{
    display: flex;
    position: relative;
    align-items: center;
    margin-top: 15px;
  }
  
  input{
    width: 100%;
    background-color:rgba(250, 248, 248);
    border: 0px;
    outline: none;
    padding: 10px;
    padding-left: 30px;
    border-radius: 10px;
  }

  .icon-input{
    position: absolute;
    margin-left: 10px;
  }
</style>
