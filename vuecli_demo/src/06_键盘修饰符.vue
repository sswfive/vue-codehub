<template>
  <div>
    <!-- 1. 绑定键盘按下事件 .enter回车-->
    <input type="text" @keydown.enter="enderFn" />
    <hr />
    <!-- 2.绑定键盘按下esc键， .esc修饰符 取消键-->
    <input type="text" @keydown.esc="escFn" />
  </div>
</template>

<script>
export default {
    methods:{
        enderFn(){
            console.log("用户按下的回车键")
        },
        escFn(){
            console.log('用户按下的是取消键')
        }
    }
}
</script>

<style>

</style>