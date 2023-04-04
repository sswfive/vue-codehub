<template>
  <div>
    <a @click="one" href="http://www.baidu.com">百度1</a>
    <hr />
    <a @click="two(10, $event)" href="http://www.taobao.com">淘宝</a>
  </div>

</template>

<script>
export default {
    methods: {
        one(e){
            e.preventDefault();
        },
        two(num, e){
            e.preventDefault();
        }
    }
}
</script>

<style>

</style>