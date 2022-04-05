<template>
    <div  :key="task.id" v-for="task in tasks">
    <Task :task = "task"/>
    </div>
</template>

<script>

import Task from '@/components/Task'

export default {
    name: 'TasksData',


    props: {
        tasks: Array
    },
    components: {
        Task
    }
    
}
</script>
