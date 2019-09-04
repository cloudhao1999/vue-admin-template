<template>
  <div class="dashboard-container">
    <div class="dashboard-text">欢迎来到vue-element-admin后台管理系统</div>
  </div>
</template>

<script>
import { mapGetters } from 'vuex'

export default {
  name: 'Dashboard',
  computed: {
    ...mapGetters([
      'name'
    ])
  }
}
</script>

<style lang="scss" scoped>
.dashboard {
  &-container {
    margin: 30px;
    height: 100%;
  }
  &-text {
    font-size: 30px;
    line-height: 46px;
    text-align: center;
    padding-top: 25%;
    color: gray;
  }
}
</style>
