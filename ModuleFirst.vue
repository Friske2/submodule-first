<template>
  <div>
    test {{msg}}
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
export default defineComponent({
  name:'ModuleFirst',
  props:{
     msg: {
      type: String,
      required: true
    }
  }
})
</script>

<style>

</style>