<template>
  <div class="expanded" :style="{flex:grow}">
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: "expanded",
  props:{
    grow: {
      type:Number,
      default:1
    },
  }
}
</script>

<style scoped>
</style>