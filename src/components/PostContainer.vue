<template>
    <div class="post_container">
        <PostCard/>
        <PostCard/>
        <PostCard/>
        <PostCard/>
    </div>


</template>

<script lang="ts" setup>
    import PostCard from './PostCard.vue';
</script>

<style scoped>

    .post_container{
        width: 100%;
        display: flex;
        flex-wrap: wrap;
    }

</style>