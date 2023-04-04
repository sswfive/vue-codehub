<template>
  <div>
    <h1>{{ msg }}</h1>
    <button @click="btn">逆转事件</button>
  </div>
</template>

<script>
export default {
    data(){
        return {
        msg: 'Welcome Hello World'
        }
    },
    methods:{
        btn(){
            //截取字符串返回数组
            let arr = this.msg.split("")
            // console.log(arr)
            //翻转
            arr.reverse()
            //数组拼接
            this.msg = arr.join("")
 
            //简写
            // this.msg = this.msg.split("").reverse().join("")
        }
    }
}
</script>

<style>

</style> 