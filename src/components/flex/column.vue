<template>
  <div class="column">
    <slot></slot>
  </div>
</template>

<script>
export default {
name: "column"
}
</script>

<style scoped>
.column{
  display: flex;
  flex-direction: column;
}
</style>