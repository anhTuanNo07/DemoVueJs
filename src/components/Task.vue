<template>
  <div class="task">
    <span>{{ taskData.content }}</span>
  </div>
</template>

<script>
export default {
    props:{
        taskData: {
            type: Object,
            default: function() { return {} }
        }
    },
    data() {
        return {
            content: 'ABC'
        }
    }
}
</script>
<style scoped>

</style>
