<template>
  <div :style="{
    fontSize:fontSize+'px',
    color:fontColor,
    fontWeight:bold?'bold':400
  }">
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: "fl-text",
  props: {
    size: {
      type: [String,Number],
      default: 14
    },
    type: {
      type: String,
      default: 'p1'
    },
    bold: {
      type: Boolean,
      default: false
    }
  },
  computed: {
    fontSize() {
      if(this.size==='h1'){
        return 20
      }else if (this.size==='h2'){
        return 18
      }else if (this.size==='h3'){
        return 16
      }else if (this.size==='p1'){
        return 14
      }else if (this.size==='p2'){
        return 13
      }else if (this.size==='p3'){
        return 12
      }else{
        return this.size
      }
    },
    fontColor() {
      return {
        default:'#303133',
        second:'#606266',
        hint:'#909399',
      }[this.type];
    }
  },
}
</script>

<style scoped>

</style>