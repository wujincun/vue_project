<template>
  <div class="panel panel-default">
    <div class="panel-heading">
      <h1 class="text-center">已有时长</h1>
    </div>

    <div class="panel-body">
      <h1 class="text-center">{{ time }} 小时</h1>
    </div>

  </div>
</template>
<style>
    body{
        background-color:#ff0000;
    }
</style>
<script>
  export default {
    name: 'sidebar',
    computed: {
      time () {
        return this.$store.state.totalTime
      }
    }
  }
</script>
