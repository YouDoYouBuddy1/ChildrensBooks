<template>
    <router-link :to = "{name: 'Inspect', params: {id :id}}" >
        <div>
           <h2>{{title}}</h2>
            <p>{{author}}</p>
        </div>
    </router-link>
</template>

<script>
export default {
    props: {
        title: String,
        author: String,
        id: Number
    }
}
</script>

<style scoped>
    div {
        background-color: grey;
        min-width: 10rem;
        min-height: 20rem;
        max-width: 20rem;
        max-height: 40rem;

        margin: 0 auto;
    }
</style>