<template>
  <div>
    <van-row type="flex" justify="center" align="center">
      <van-col span="18">
        <van-form @submit="onSubmit">
          <van-field
            v-model="username"
            name="用户名"
            label="用户名"
            placeholder="用户名"
            :rules="[{ required: true, message: '请填写用户名' }]"
          />
          <van-field
            v-model="password"
            type="password"
            name="密码"
            label="密码"
            placeholder="密码"
            :rules="[{ required: true, message: '请填写密码' }]"
          />
          <div style="margin: 16px;">
            <van-button round block color="linear-gradient(to right, #4bb0ff, #6149f6)" size="small" native-type="submit" to="/">
              提交
            </van-button>
          </div>
        </van-form>
      </van-col>
    </van-row>
  </div>
</template>

<script>
export default {
  name: 'Login',
  data() {
    return {
      username: '',
      password: ''
    }
  },
  components: {},
  created() {},
  mounted() {},
  methods: {
    onSubmit(values) {
      console.log('submit', values)
    }
  },
  computed: {}
}
</script>

<style scoped lang="scss"></style>
