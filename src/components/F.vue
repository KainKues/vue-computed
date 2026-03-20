<script>
import {ref, computed} from 'vue'
let name = ref('')
let alertMes = computed(()=> {
    return `Привет, ${name.value}!`
})

</script>

<template>
    <input type="text"
            class="input"
            v-model = 'name'>
    <div class="message"
            v-if="name">{{ alertMes }}</div>
            
</template>

<style>
    .message{
        background-color: white;
        color: black;
        width: 200px;
        height: 20px;
    }
</style>