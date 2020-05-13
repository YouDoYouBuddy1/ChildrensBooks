<template>
    <router-link :to = "'/'" >
        <div>
           <h2>{{title}}</h2>
            <p>{{author}}</p>
            <p>{{plot}}</p>
        </div>
    </router-link>
</template>

<script>
export default {
    props: {
        title: String,
        author: String,
        plot: String,
        id: Number
    }
}
</script>

<style scoped>
    div {
        background-color: green;
        min-width: 20rem;
        min-height: 30rem;
        max-width: 50rem;
        max-height: 70rem;

        margin: 0 auto;
    }
</style>