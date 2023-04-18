<script lang="ts">
  export default {
    name: 'Navbar',
  };
</script>

<template>
    <div class="w-full bg-indigo-950 text-white px-6 py-5 flex justify-between items-center border-b border-purple-600 fixed z-10 shadow-md">
        <div>logo</div>
        <div class="flex gap-2">
            <button class="px-4 py-3 rounded-lg font-semibold border bg-purple-800 border-purple-950 hover:bg-purple-950 ease-in-out duration-300 ">Entrar</button>
            <button class="px-6 py-3 rounded-lg font-semibold border bg-purple-600 border-purple-800 hover:bg-purple-800 ease-in-out duration-300 ">Cadastrar</button>
        </div>
    </div>
</template>