<template>
    <div class="post_card">
      <h3>Título</h3>
    <p>Descripción</p>  

    <PostButton/>

    </div>

</template>

<script lang="ts" setup>
    import PostButton from './PostButton.vue';

</script>

<style scoped>
    .post_card {
        border-radius: 15px;
        padding: 10px;
        margin: 5px;
        border: 1px solid #ccc
    }
</style>