<template>
  <div>
    {{msg}} {{count}}
    <button @click="handleEvent">count</button>
  </div>
</template>

<script lang="ts">
import { ref,defineComponent } from 'vue'
export default defineComponent({
  name:'ModuleFirst',
  props:{
     msg: {
      type: String,
      required: true
    }
  },
  setup:()=> {
    let count = ref(0)
    const handleEvent = ()=> {
      count.value++
    }
    return { count,handleEvent }
  }
})
</script>

<style>

</style>