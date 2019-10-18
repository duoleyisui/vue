<template>
<div>
    <van-cell-group class="juzhong">
  <van-field class="inputarea"
    v-model="username"
    required
    clearable
    label="用户名"
    right-icon="question-o"
    placeholder="请输入用户名"
    @click-right-icon="$toast('question')"
  />

  <van-field
    v-model="password" class="inputarea"
    type="password"
    label="密码"
    placeholder="请输入密码"
    required
  />
</van-cell-group>
<div>
    <router-link to="/home"><van-button type='primary'>登录</van-button></router-link>
</div>
</div>
   

</template>
<script>
export default {
    data(){
        return{
            username:'',
            password:''
        }
    }
}
</script>
<style lang="scss" scoped>
.juzhong{
    text-align: center;
}

</style>