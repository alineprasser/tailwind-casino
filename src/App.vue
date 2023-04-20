<script setup>
import MainPage from "./components/MainPage.vue";
import Navbar from "./components/Navbar.vue";
import Sidebar from "./components/Sidebar.vue";
</script>

<template>
  <div class="flex flex-col">
    <header>
      <Navbar />
    </header>
    <main class="flex justify-between">
      <aside class="relative">
        <Sidebar class="sticky top-0 h-screen" />
      </aside>
      <article class="w-full">
        <MainPage />
      </article>
    </main>
    <footer></footer>
  </div>
</template>
