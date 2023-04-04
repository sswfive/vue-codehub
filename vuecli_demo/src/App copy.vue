<template>
  <div>
    <div>
        <span>年龄：</span>
        <!-- number修饰符 把值parseFloat转成数值类型  -->
        <input type="number" v-model.number="age">
    </div>
    <div>
        <span>人生格言</span>
        <!-- trim 去除左右两边空格后把值付给vue数据变量 -->
        <input type="text" v-model.trim="motto">
    </div>
    <div>
        <span>个人简介</span>
        <!-- lazy 等表单是去焦点，才把值赋值给vue数据变量 -->
        <textarea v-model.lazy ="intro"></textarea>
    </div>
  </div>
</template>

<script>
export default {
    data(){
        return {
            age: 0,
            motto: '',
            intro: '',
        }
    }

}
</script>

<style>

</style>