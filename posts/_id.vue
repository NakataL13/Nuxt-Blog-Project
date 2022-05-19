<template>
    <div>
        <PostsTable
        v-for="post in posts"
        :key="id"
        />
    </div>
</template>

<script>
import Posts from './index.vue'
    export default{
    data() {
        return {
            props: ["id", "title", "body", "posts"]
        };
    },
    components: { Posts }
}

</script>