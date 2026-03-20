<script>
import {ref, computed} from 'vue'
let text = ref('')
let sum = computed(()=> {
    return text.value.length;
})

</script>

<template>
    <input type="text"
            class="input"
            v-model = 'text'>
    <div class="message"
            v-if="sum">Количество символов: {{ sum }}</div>
            
</template>

<style>
    .message{
        background-color: white;
        color: black;
        width: 200px;
        height: 20px;
    }
</style>