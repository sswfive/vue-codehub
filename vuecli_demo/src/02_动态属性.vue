<template>
    <div>
        <a v-bind:href="url">百度链接</a>
        <img :src="imgUrl">
    </div>
  
</template>

<script>
export default {
    data(){
        return {
            url:'http://www.baidu.com',
            imgUrl: "https://static.runoob.com/images/demo/demo2.jpg"
        }
    }

}
</script>

<style>

</style>