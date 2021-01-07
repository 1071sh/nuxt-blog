<template>
    <section class="post-list">
        <PostPreview
            :is-admin="isAdmin"
            id="1"
            title="Hello"
            previewText="This my first post!"
            thumbnail="https://static.pexels.com/photos/270348/pexels-photo-270348.jpeg"
        />
        <PostPreview
            :is-admin="isAdmin"
            id="2"
            title="Hello"
            previewText="This my first post!"
            thumbnail="https://static.pexels.com/photos/270348/pexels-photo-270348.jpeg"
        />
        <PostPreview
            :is-admin="isAdmin"
            id="3"
            title="Hello"
            previewText="This my first post!"
            thumbnail="https://static.pexels.com/photos/270348/pexels-photo-270348.jpeg"
        />
    </section>
</template>

<script>
import PostPreview from "@/components/Posts/PostPreview";
export default {
    components: {
        PostPreview
    },
    props: {
        isAdmin: {
            type: Boolean,
            default: false
        }
    }
};
</script>

<style scoped>
.post-list {
    display: flex;
    padding: 20px;
    box-sizing: border-box;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
}
</style>
