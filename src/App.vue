<template>
  <div class="block">
    <span class="demonstration">指示器</span>
    <el-carousel height="150px" interval="2000" type="card">
      <el-carousel-item v-for="(item,index) in 3" :key="item">
        <img
          src="https://pic4.zhimg.com/v2-3be05963f5f3753a8cb75b6692154d4a_1200x500.jpg"
          v-if="index == 0"/>
        <img
          src="http://img.netbian.com/file/2019/0426/c1dfac463602581d897d4f13280358f2.jpg"
          v-if="index == 1"
        />
        <img
          src="https://p.bigstockphoto.com/GeFvQkBbSLaMdpKXF1Zv_bigstock-Aerial-View-Of-Blue-Lakes-And--227291596.jpg"
          v-if="index == 2"
        />
      </el-carousel-item>
    </el-carousel>
  </div>
</template>

<style>
.el-carousel__item img {
  display: inline-block;
  height: 100%;
  width: 100%;
  object-fit: cover;
}
.el-carousel__item:nth-child(2n) {
  background-color: #99a9bf;
}

.el-carousel__item:nth-child(2n + 1) {
  background-color: #d3dce6;
}
</style>
