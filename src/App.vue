<script setup>
import MainPage from "./components/MainPage.vue";
import Navbar from "./components/Navbar.vue";
import Sidebar from "./components/Sidebar.vue";
import Foot from "./components/Foot.vue";
</script>

<template>
  <div class="">
    <header>
      <Navbar />
    </header>
    <div class="flex">
      <aside class="sticky top-0 h-full">
        <Sidebar class="" />
      </aside>
      <main class="w-full">
        <article>
          <MainPage />
        </article>
      </main>
    </div>
    <footer><Foot /></footer>
  </div>
</template>
