<template>
  <div class="container">
    <h2>BẢNG THỐNG KÊ</h2>
    <div class="thongke">
      <!-- trái -->
      <!-- 1 -->
      <div class="thong-ke__list bg__section">
        <div class="thong-ke__soluong">
          <h2 class="thong-ke__dem">25,119</h2>
          <img src="" alt="" />
        </div>
        <p class="thong-ke__content">Số người thăm thư viện</p>
      </div>
      <!-- 2 -->
      <div class="thong-ke__list bg__section">
        <div class="thong-ke__soluong">
          <h2 class="thong-ke__dem">33.17%</h2>
          <img src="" alt="" />
        </div>
        <p class="thong-ke__content">Sách mượn</p>
      </div>
      <!-- 3 -->
      <div class="thong-ke__list bg__section">
        <div class="thong-ke__soluong">
          <h2 class="thong-ke__dem">25,119</h2>
          <img src="" alt="" />
        </div>
        <p class="thong-ke__content">Sách quá hạn</p>
      </div>
      <!-- phải -->
    </div>
  </div>
</template>
<script setup lang="ts"></script>

<style scoped>
/* thuộc tính chung */
.bg__section {
  background-color: #f5f5f5;
}
/* -----------------thống kê-------------------- */
.thongke {
  width: 20%;
  display: flex;
  flex-direction: column;
  row-gap: 25px;
}
.thong-ke__list {
  padding: 12%;
  border-radius: 15px;
}
</style>
