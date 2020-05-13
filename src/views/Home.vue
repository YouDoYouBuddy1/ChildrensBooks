<template>
  <div class="home">
    <section class = "books"
    v-for="b in books"
    v-bind:key=b.id>
      <book v-bind:title = "b.title"
      v-bind:author = "b.author"
      v-bind:id = "b.id"/>
    </section>
  </div>
</template>

<script>
// @ is an alias to /src
import book from '@/components/book.vue'
import json from './childrensbooks.json'

export default {
  name: 'Home',
  data: function(){
    return {
      books: json.books
    }
  },
  components: {
    book
  }
}
</script>

<style scoped>
  .home {
    display: grid;
    grid-template: 10vw / auto auto auto auto;
  }
</style>
