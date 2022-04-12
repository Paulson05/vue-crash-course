
<template>
  <button @click="onClick()"  :style="{backgound:color}" class="btn" >{{ text }}</button>
</template>

<script>
export default {
  name: 'ButtonTask',
  props: {
    text: String,
    color: String
  },
  methods: {
    onClick () {
       this.$emit('toggle-add-task')
     
    }
  }
}
</script>
