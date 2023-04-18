<script lang="ts">
    import { Camera } from 'lucide-vue-next';

  export default {
    name: 'Sidebar',
    components: { Camera }
  };
</script>

<template>
    <div class="flex flex-col min-h-screen bg-indigo-950 text-white w-60 py-24 fixed border-r border-purple-950 ">
        <div class="flex w-full border-b-2 border-purple-950">
            <button class="p-2 font-bold w-full border-b-2 border-purple-800" >Casino</button>
            <button class="p-2 font-bold w-full ">Sports</button>
        </div>
        <nav class="px-6 py-4">
            <ul class="flex flex-col gap-3">
                <li class="border border-white/10 rounded-md px-2 py-3 font-semibold text-sm bg-transparent hover:bg-white/5 ease-in-out duration-150 cursor-pointer"><p>Início</p></li>
                <li class="border border-white/10 rounded-md px-2 py-3 font-semibold text-sm bg-transparent hover:bg-white/5 ease-in-out duration-150 cursor-pointer"><p>Depositar</p></li>
                <li class="border border-white/10 rounded-md px-2 py-3 font-semibold text-sm bg-transparent hover:bg-white/5 ease-in-out duration-150 cursor-pointer"><p>Sacar</p></li>
            </ul>
        </nav>
    </div>
</template>
