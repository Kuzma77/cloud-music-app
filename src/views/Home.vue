<template>
  <div>
    <van-nav-bar border fixed @click-left="onClickLeft" @click-right="onClickRight">
      <template #left>
        <van-icon name="contact" size="18" />
      </template>
      <template #right>
        <van-icon name="search" size="18" />
      </template>
      <template #title>
        <van-row gutter="20" type="flex" justify="center">
          <van-col span="6">我的</van-col>
          <van-col span="6">发现</van-col>
          <van-col span="6">云村</van-col>
          <van-col span="6">视频</van-col>
        </van-row>
      </template>
    </van-nav-bar>
  </div>
</template>

<script>
import { Toast } from 'vant'
export default {
  name: 'Home',
  data() {
    return {}
  },
  components: {},
  created() {},
  mounted() {},
  methods: {
    onClickLeft() {
      Toast('返回')
    },
    onClickRight() {
      Toast('按钮')
    }
  },
  computed: {}
}
</script>

<style scoped lang="scss"></style>
