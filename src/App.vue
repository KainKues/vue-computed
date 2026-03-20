<script setup>  
  import F from "./components/F.vue"
  import S from "./components/S.vue"
</script>
 
<template>
  <div class="field">
    <div class="block">
      <F></F>
    </div>
    <div class="block">
      <S></S>
    </div>
  </div>
</template>

<style>
  body{
    background-color: gray;
  }
  .field{
    display: flex;
    flex-direction: column;
    gap: 40px
  }

</style>
