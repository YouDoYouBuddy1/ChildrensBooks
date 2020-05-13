<template>
  <div class="inspect">
    <bigBook v-bind:title = "books[$route.params.id - 1].title"
    v-bind:author = "books[$route.params.id - 1].author"
    v-bind:id = "books[$route.params.id - 1].id"
    v-bind:plot = "books[$route.params.id - 1].plot"/>
  </div>
</template>

<script>
import bigBook from '@/components/bigBook.vue'
import json from './childrensbooks.json'

export default {
  name: 'Inspect',
  data: function(){
    return {
      books: json.books
    }
  },
  components: {
    bigBook
  }
}
</script>
