<script lang="ts" setup>
interface Book {
  title: string;
  language: string;
  rank: string;
}

const url = 'https://edwardtanguay.vercel.app/share/books.json';

const { data: books } = useFetch<Book[]>(url);
</script>

<template>
  <div>
    <h1>There are {{ books?.length }} books available</h1>
    <ul>
      <li v-for="book in books" :key="book.title">
        {{ book.title }} ({{ book.language }}) - {{ book.rank }}
      </li>
    </ul>
  </div>
</template>
