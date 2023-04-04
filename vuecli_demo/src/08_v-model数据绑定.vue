<template>
  <div>
    <div>
        <span>用户名：</span>
        <!-- 
            v-model 双向数据绑定 
            value属性 - vue变量
        -->
        <input type="text" v-model="username" />
    </div>
    <div>
        <span>密  码：</span>
        <input type="password" v-model="password" />
    </div>
  </div>
</template>

<script>
export default {
    data(){
        return {
            username: "",
            password: ""
        }
    }
}
</script>

<style>

</style>