<template>
  <div>
    <div>
        <span>来自于：</span>
        <!-- 下拉菜单 v-model 写在select value在option上 -->
        <select v-model="form">
            <option value="北京">北京</option>
            <option value="南京">南京</option>
            <option value="天津">天津</option> 
        </select>
    </div>
    <div>
        <!-- 
            遇到复选框， v-model 的变量值
            非数组 - 关联的事复选框的checked 属性
            数组 - 关联的事复选框的value属性
         -->
        <span>爱好：</span>
        <input type="checkbox" v-model="hobby" value="篮球">篮球
        <input type="checkbox" v-model="hobby" value="吃饭">吃饭
        <input type="checkbox" v-model="hobby" value="睡觉">睡觉
    </div>
    <div>
        <span>性别：</span>
        <input type="radio" value="男" v-model="gender" name="sex">男
        <input type="radio" value="女" v-model="gender" name="sex">女

    </div>
    <div>
        <span>自我介绍</span>
        <textarea v-model="intro"></textarea>
    </div>
  </div>
</template>

<script>
export default {
    data(){
        return {
            form: '',
            hobby: [],
            gender: '男',
            intro:'',
        }
    }
}
</script>

<style>

</style>