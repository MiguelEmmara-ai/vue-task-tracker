<template lang="">
     <div>
          <button @click="onClick()" :style="{background: color}" class="btn">{{ text }}</button>
     </div>
</template>

<script>
export default {
     name: 'Button',
     props: {
          text: {
               type: String,
               default: 'Add Task',
          },

          color: {
               type: String,
               default: 'green',
          },
     },
     methods: {
          onClick() {
               console.log('click');
          }
     }
}
</script>

<style scoped>
     
</style>