<template>
  <div>
    <el-row>
      <el-button type="info" @click="logout">退出</el-button>
    </el-row>
  </div>
</template>

<script>
export default {
  data () {
    return {}
  },
  created () {},
  methods: {
    logout () {
      window.sessionStorage.clear()
      this.$router.push('/login')
    }
  }
}
</script>

<style lang="less" scoped></style>
