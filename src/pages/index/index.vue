<template>
  <div class="containerBox">
    <div class="innerBox">
      <div class="titleBox">subEditor</div>
      <div class="contentBox">
        <div class="row" v-for="(subFile,i) in subFiles" :key="i">
          <label class="left">
            <img class="img" src="../../../static/tabs/file.png" alt="文件" />
            <span class="fileName">{{subFile.fileName}}</span>
          </label>
          <label class="rightText">
            <span>></span>
          </label>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      subFiles: [{ fileName: "name.vtt" }, { fileName: "qy.vtt" }]
    };
  }
};
</script>

<style lang="scss" scoped>
.containerBox {
  display: flex;
  height: 100vh;
  width: 100vw;
  justify-content: center;
  align-items: center;
  flex-flow: column nowrap;
  .innerBox {
    flex:1;
    width: 100%;
    display: flex;
    flex-direction: column;
    .titleBox {
      text-align: center;
      margin: 30px;
      font-size: 30px;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      font-style: italic;
      color: #66cccc;
    }
    .contentBox {
      .rightText {
        clear: right;
        float: right;
        height: 55px;
        color: #E8E8E8;
      }
      .row {
        height: 55px;
        border-bottom: 1px #E8E8E8 solid;
        line-height: 70px;
        padding: 0 20px;
        .img {
          width: 30px;
          height: 30px;
          float: left;
          padding-top: 20px;
        }
        .fileName {
          margin-left: 10px;
        }
      }
    }
  }
}
</style>
