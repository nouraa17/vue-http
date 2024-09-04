<template>
  <div>
    <button @click="incrementCount"> Clicked {{count}} Times</button>
  </div>
</template>

<script>
import CounterMixins from "@/mixins/counter";
  export default {
    name: 'ClickCounter',
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