<script lang="ts">
import {
  Home,
  DollarSign,
  ArrowDown,
  GiftIcon,
  UserIcon,
  Shovel,
  Component,
  Share,
  Instagram,
} from "lucide-vue-next";

export default {
  name: "Sidebar",
  components: {
    Home,
    DollarSign,
    ArrowDown,
    GiftIcon,
    UserIcon,
    Shovel,
    Component,
    Instagram,
    Share,
  },
};
</script>

<template>
  <div
    class="sm:flex sm:flex-col hidden bg-zinc-900 text-white w-60 pt-20 pb-10 border-r sticky border-purple-950"
  >
    <div class="flex w-full border-b-2 border-purple-950">
      <button class="p-2 font-bold w-full border-b-2 border-purple-800">
        Casino
      </button>
      <button class="p-2 font-bold w-full">Sports</button>
    </div>
    <div>
      <nav class="px-6 py-5">
        <ul class="flex flex-col gap-2">
          <li
            class="border border-white/10 rounded-md px-4 py-3 text-sm bg-white/5 hover:bg-white/10 ease-in-out duration-150 cursor-pointer flex gap-4 items-center"
          >
            <Home :size="16" class="text-purple-800" />
            <p class="text-purple-800 font-bold">Início</p>
          </li>
          <li
            class="border border-white/10 rounded-md px-4 py-3 text-sm bg-transparent hover:bg-white/5 ease-in-out duration-150 cursor-pointer flex gap-4 items-center"
          >
            <DollarSign :size="16" class="text-purple-800" />
            <p class="text-white/40 font-semibold">Depositar</p>
          </li>
          <li
            class="border border-white/10 rounded-md px-4 py-3 text-sm bg-transparent hover:bg-white/5 ease-in-out duration-150 cursor-pointer flex gap-4 items-center"
          >
            <ArrowDown :size="16" class="text-purple-800" />
            <p class="text-white/40 font-semibold">Sacar</p>
          </li>
        </ul>
      </nav>
    </div>
    <div class="border-b border-white/10 mx-6 my-4"></div>
    <div class="px-6 my-4">
      <ul class="flex flex-col gap-2">
        <li
          class="border border-purple-800 flex items-center transition-all gap-3 bg-gradient-to-br from-purple-900 px-3 py-3 font-semibold rounded-sm hover:from-purple-700 hover:to-zinc-950 ease-in-out duration-500 cursor-pointer"
        >
          <div class="w-6 h-6 bg-white/50 rounded-full"></div>
          <p>Grau</p>
          <sup class="pl-3 text-zinc-400 text-xs font-semibold">New!</sup>
        </li>
        <li
          class="border border-purple-800 flex items-center transition-all gap-3 bg-gradient-to-br from-purple-900 px-3 py-3 font-semibold rounded-sm hover:from-purple-700 hover:to-zinc-950 ease-in-out duration-500 cursor-pointer"
        >
          <div class="w-6 h-6 bg-white/50 rounded-full"></div>
          <p>Gold Crash</p>
        </li>
        <li
          class="border border-purple-800 flex items-center transition-all gap-3 bg-gradient-to-br from-purple-900 px-3 py-3 font-semibold rounded-sm hover:from-purple-700 hover:to-zinc-950 ease-in-out duration-500 cursor-pointer"
        >
          <div class="w-6 h-6 bg-white/50 rounded-full"></div>
          <p>Double</p>
        </li>
        <li
          class="border border-purple-800 flex items-center transition-all gap-3 bg-gradient-to-br from-purple-900 px-3 py-3 font-semibold rounded-sm hover:from-purple-700 hover:to-zinc-950 ease-in-out duration-500 cursor-pointer"
        >
          <div class="w-6 h-6 bg-white/50 rounded-full"></div>
          <p>Dice</p>
        </li>
        <li
          class="border border-purple-800 flex items-center transition-all gap-3 bg-gradient-to-br from-purple-900 px-3 py-3 font-semibold rounded-sm hover:from-purple-700 hover:to-zinc-950 ease-in-out duration-500 cursor-pointer"
        >
          <div class="w-6 h-6 bg-white/50 rounded-full"></div>
          <p>Mines</p>
        </li>
      </ul>
    </div>
    <div class="border-b border-white/10 mx-6 my-2"></div>
    <div>
      <div class="px-6 py-5">
        <ul class="flex flex-col gap-2">
          <li
            class="border border-white/10 rounded-md px-4 py-3 text-sm bg-transparent hover:bg-white/5 ease-in-out duration-150 cursor-pointer flex gap-4 items-center"
          >
            <GiftIcon :size="16" class="text-purple-800" />
            <p class="text-white/40 font-semibold">Promoções</p>
          </li>
          <li
            class="border border-white/10 rounded-md px-4 py-3 text-sm bg-transparent hover:bg-white/5 ease-in-out duration-150 cursor-pointer flex gap-4 items-center"
          >
            <UserIcon :size="16" class="text-purple-800" />
            <p class="text-white/40 font-semibold">Minha Conta</p>
          </li>
          <li
            class="border border-white/10 rounded-md px-4 py-3 text-sm bg-transparent hover:bg-white/5 ease-in-out duration-150 cursor-pointer flex gap-7 items-center"
          >
            <div
              class="w-11 h-11 bg-purple-800 rounded-r-full rounded-l-md absolute left-6 z-[-1]"
            ></div>
            <Shovel :size="16" class="text-white" />
            <p class="text-white/40 font-semibold">Baú de Tesouros</p>
          </li>
          <li
            class="border border-white/10 rounded-md px-4 py-3 text-sm bg-transparent hover:bg-white/5 ease-in-out duration-150 cursor-pointer flex gap-7 items-center"
          >
            <div
              class="w-11 h-11 bg-purple-800 rounded-r-full rounded-l-md absolute left-6 z-[-1]"
            ></div>
            <Component :size="16" class="text-white" />
            <p class="text-white/40 font-semibold">Seja sócio</p>
          </li>
        </ul>
      </div>
    </div>
    <div class="border-b border-white/10 my-4"></div>
    <div class="flex flex-col gap-3 mx-6 text-zinc-500 text-xs mt-4">
      <div class="flex gap-3">
        <Instagram
          :size="14"
          class="hover:text-zinc-300 cursor-pointer ease-in-out duration-300"
        />
        <Share
          :size="14"
          class="hover:text-zinc-300 cursor-pointer ease-in-out duration-300"
        />
      </div>
      <p class="">© 2023, All right reserved</p>
    </div>
  </div>
</template>
