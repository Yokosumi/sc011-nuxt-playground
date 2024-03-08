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
    <h1 class="text-xl">
      There are
      <span class="font-bold text-green-400">{{ books?.length }}</span> books
      available
    </h1>
    <ul>
      <li
        v-for="book in books"
        :key="book.title"
        class="my-2 border-2 max-w-fit-content p-2 rounded-md bg-gradient-to-l from-gray-500 to-blue-200"
      >
        <p>Title: {{ book.title }}</p>
        <p>Language: {{ book.language }}</p>
        <p>Rank: {{ book.rank }}</p>
      </li>
    </ul>
  </div>
</template>
