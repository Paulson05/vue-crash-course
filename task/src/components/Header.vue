<template>
  <header>
    <h1>{{title }}</h1>
      <Button @toggle-add-task= "$emit('toggle-add-task')"  text= "add task" color= "green"/>
  </header>

</template>

<script>
import Button from '@/components/Button'

export default {
  name: 'HeaderTask',
  props: {
    title: String
  },
  components: {
    Button
  }
}
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}

.btn {
  display: inline-block;
  background: rgb(79, 247, 101);
  color: #fff;
  border: none;
  padding: 10px 20px;
  margin: 5px;
  border-radius: 5px;
  cursor: pointer;
  text-decoration: none;
  font-size: 15px;
  font-family: inherit;
}

</style>
