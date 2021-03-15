<template>
  <div class="center">
    <slot></slot>
  </div>
</template>

<script>
export default {
name: "fl-center"
}
</script>

<style scoped>
.center{
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>