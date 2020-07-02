<template>
  <div class="container">
    <div class="innerBox">
      <div class="boxTitle">
        mpvue小程序
      </div>
      <div class="boxContent">
        内容
      </div>
    </div>
  </div>
</template>

<script></script>

<style lang="scss" scoped>
.container {
  display: flex;
  height: 100vh;
  width: 100vw;
  justify-content: center;
  align-items: center;
  .innerBox {
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: center;
    .boxTitle {
      font-weight: bold;
      font-size: 24px;
      margin-bottom: 30vh;
    }
    .boxContent {
      justify-content: center;
      align-items: center;
    }
  }
}
</style>
