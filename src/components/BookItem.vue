<template>
  <li>
    {{book.title}} : {{book.author}}
    <span v-if="book.finishReading == true">Read</span>
    <span v-else>Not Read</span>
  </li>
</template>

<script>
import BookList from './BookList'
export default {
  
  name: 'BookItem',
  props: ['book'],
  components:{
    BookList,
  }
};
</script>

<style>
li {
  display: block;
  margin: 0 10px;
}
</style>