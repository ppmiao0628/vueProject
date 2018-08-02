<template>
  <div class="wrap">
    在下是弹窗
  </div>
</template>

<script>
export default {
  name: 'toast',
  data: function () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .wrap {
    position: fixed;
    left: 50%;
    top: 50%;
    background: rgba(0, 0, 0, .35);
    padding: 10px;
    -webkit-border-radius: 5px;
    -moz-border-radius: 5px;
    border-radius: 5px;
    -webkit-transform: translate(-50%, -50%);
    -moz-transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
    -o-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
    color: #fff;
  }
</style>
