<template>
    <div>
        <!--赋值到标签-->
        <h1>{{ msg }}</h1>
        <h2>{{ obj.name }}</h2>
        <h3>{{ obj.age >= 18 ? "成年" : "未成年" }}</h3>
    </div>
</template>

<script>
export default {
    // 1. 变量在data函数的return对象上
    data() {
        return {
            msg: 'Hello, Vue',
            obj: {
                name: '小vue',
                age: 5
            }
        }
    }

}
</script>

<style>

</style>