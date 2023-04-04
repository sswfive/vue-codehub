<template>
  <div>
    <p>你要购买的商品数量为{{ count }}</p>
    <!--1. 绑定事件  语法： v-on: 事件名=“少量代码-->
    <button v-on:click="count = count + 1 ">+1</button>
    
    <!--2.语法： v-on: 事件名=“methods里的函数名”-->
    <button v-on:click = "addFn">+1</button>
    
    <!--3.语法： v-on:事件名=“methods函数名（值）”-->
    <button v-on:click = "addCountFn(10)">+10</button>

    <!--4.简写 @click-->
    <button @click = "subFn">-1</button>
  </div>


</template>

<script>
export default {
    data() {
        return {
            count: 1,
        }
    },
    methods: {
        addFn(){
            // this指向的export dfault的{}
            this.count ++
        },
        addCountFn(num){
            this.count = this.count + num
        },
        subFn(){
            this.count--
        }
    }

}
</script>

<style>

</style>