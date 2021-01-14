<template>
  <div class="x-button" @click="btnClick">
    <slot></slot>
  </div>
</template>
<script>
export default {
  name: 'x-button',
  props: {
    type: String
  },
  methods:{
    btnClick(){
      alert('111')
    }
  }
}
</script>
 
<style scoped>
  .x-button {
      display: inline-block;
      padding: 3px 6px;
      background: #000;
      color: #fff;
  }
</style>
