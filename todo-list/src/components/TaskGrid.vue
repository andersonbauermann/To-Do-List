<template>
    <div class="tasks-grid">
        <template>
            <task v-for="task in tasks" :key="task.name" :task="task">
            </task>
        </template>
    </div>
</template>

<script>

import Task from './Task.vue';

export default {
    components: { Task },
    props: {
        tasks: {
            type: Array,
            required: true
        }
    }
}
</script>
