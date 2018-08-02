<template>
  <div class="wrap" v-if="showWrap" :class="showContent?'fadein':'fadeout'">
    {{text}}
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
  .fadein {
    -webkit-animation: animate_in 0.25s;
    -o-animation: animate_in 0.25s;
    animation: animate_in 0.25s;
  }
  .fadeout {
    -webkit-animation: animate_out 0.25s;
    -o-animation: animate_out 0.25s;
    animation: animate_out 0.25s;
    opacity: 0;
  }
  @keyframes animate_in {
    0% {
      opacity: 0;
    }
    100%{
      opacity: 1;
    }
  }
  @keyframes animate_out {
    0% {
      opacity: 1;
    }
    100%{
      opacity: 0;
    }
  }
</style>
