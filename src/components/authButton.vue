<template>
  <div class="btnpadding">
    <div class="button" @click="sendClick">{{ text }}</div>
  </div>
</template>

<script>
export default {
  props: ["text"],
  methods: {
    sendClick() {
      this.$emit("clickbtn");
      // console.log("子组件发送事件");
    }
  }
};
</script>

<style lang="less" scoped>
.btnpadding {
  padding: 6.389vw;
  padding-bottom: 0;
  .button {
    width: 100%;
    height: 13.889vw;
    line-height: 13.889vw;
    border-radius: 13.889vw;
    // box-sizing: border-box;
    outline: none;
    border: none;
    background-color: rgb(252, 98, 124);
    text-align: center;
    color: #fff;
    font-size: 4.444vw;
  }
}
</style>
