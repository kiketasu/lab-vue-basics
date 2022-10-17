<template>
    <div v-for="element in data" >{{element.title}}, {{element.description}}, {{element.content}}</div>
</template>
<script setup>
const data = [
    {
        title: 'titulo1',
        description: 'lore ipsum',
        content: 'content1'
    },
    {
        title: 'titulo2',
        description: 'lore ipsum',
        content: 'content2'
    },
    {
        title: 'titulo3',
        description: 'lore ipsum',
        content: 'content3'
    }
]
</script>
<style scoped>
</style>