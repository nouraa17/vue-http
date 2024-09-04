<template>
  <div>
    <h2 @mouseover="incrementCount"> Hovered {{count}} Times</h2>
  </div>
</template>

<script>
import CounterMixins from "@/mixins/counter";
  export default {
    name: 'HoverCounter',
    // data(){
    //   return{
    //     count:0,
    //   }
    // },
    // methods:{
    //   incrementCount(){
    //     this.count += 1;
    //   }
    // },
    mixins:[CounterMixins],
  }
</script>

<style scoped>

</style>