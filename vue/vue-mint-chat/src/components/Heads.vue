<template lang="html">
  <section class="top">
    <img src="../assets/default.png"
     alt="" class="head">
    <span class="name">客服MM</span>
    <span class="voice">
      <i class="fa"
      :class="voiceOpen?'fa-volume-up':'fa-volume-down'"
      v-on:click="voiceOpen=voiceOpen?false:true"
      aria-hidden="true"></i>
    </span>
  </section>
</template>

<script>
export default {
  data () {
    return {
      voiceOpen: true
    }
  }
}
</script>

<style lang="css" scoped>
.top {
  height: 50px;
  line-height: 50px;
  position: absolute;
  top: 0px;
  left: 0px;
  right: 0px;
  background-color: #F8F8F8;
  padding: 5px 10px;
}

.top .head {
  width: 50px;
  height: 50px;
  float: left;
  border-radius: 100%;
}

.top .name {
  font-size: 18px;
  color: #444;
  margin-left: 10px;
}

.top .voice {
  width: 30px;
  height: 50px;
  float: right;
  text-align: center;
}
</style>
