<template>
<h1>Pages</h1>
    <div v-if="pages.length">
    <div v-for="page in pages" :key="page.id" class="page">
    <h2>{{ page.title.rendered }} </h2>
<div class="post-content" v-html="page.content.rendered"></div>
    </div></div>
    <div v-else>
        <p>loading pages...</p>
    </div>
</template>

<script>
export default {
    data() {
        return {
            pages: []
        }
    },
    mounted() {
        fetch('https://www.liamjken.com/wp-json/wp/v2/posts')
        .then(res => res.json())
        .then(data => this.pages = data)
        .catch(err => console.log(err.message))
    }
}
</script>

<style>
</style>