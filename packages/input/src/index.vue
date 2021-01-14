<template>
  <div class="x-input">
    <input type="text" :value="value" @input="change($event.target.value)">
  </div>
</template>
<script>
export default {
  name: 'x-input',
  model:{
    prop: 'value',
    event: 'inputEvt'
  },
  props: {
    value: [String, Number]
  },
  methods:{
    change(val){
      this.$emit('inputEvt',val)
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
