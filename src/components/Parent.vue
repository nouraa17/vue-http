<template>
  <div>
    <h2>Parent Component</h2>
    <button @click="showChild = !showChild">Toggle button</button>
    <Child v-if="showChild"></Child>
  </div>
</template>

<script>
import Child from "@/components/Child.vue";
  export default {
    name:'ParentComponent',
    components:{
      Child,
    },
    data(){
      return{
        showChild:true,
      }
    },
    beforeCreate(){
      console.log('Parent beforeCreate')
    },
    created(){
      console.log('Parent created')
    },
    beforeMount() {
      console.log('Parent beforeMount')
    },
    mounted() {
      console.log('Parent mounted')
    },
    beforeUpdate() {
      console.log('Parent beforeUpdate')
    },
    updated() {
      console.log('Parent updated')
    },
    beforeUnmount() {
      console.log('Parent beforeUnmount')
    },
    unmounted() {
      console.log('Parent unmounted')
    },

  }
</script>

<style scoped>

</style>