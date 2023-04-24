<script lang="ts">
import { Gamepad2 } from "lucide-vue-next";
import { Trophy } from "lucide-vue-next";
import { Joystick } from "lucide-vue-next";
import { Component } from "lucide-vue-next";
import Button from "./Button.vue";

export default {
  name: "MainPage",
  components: { Component, Joystick, Gamepad2, Trophy, Button },
};
</script>

<template>
  <div
    class="mt-28 mx-auto w-4/5 overflow-x-hidden mb-5 flex flex-col justify-center"
  >
    <div class="grid lg:grid-cols-3 grid-cols-1 gap-2">
      <div
        class="w-full h-[280px] rounded-md bg-purple-300 hover:bg-purple-200 hover:shadow-md hover:shadow-zinc-400 transition-all ease-in-out duration-150 cursor-pointer"
      ></div>
      <div
        class="w-full h-[280px] rounded-md bg-purple-300 hover:bg-purple-200 hover:shadow-md hover:shadow-zinc-400 transition-all ease-in-out duration-150 cursor-pointer"
      ></div>
      <div
        class="w-full h-[280px] rounded-md bg-purple-300 hover:bg-purple-200 hover:shadow-md hover:shadow-zinc-400 transition-all ease-in-out duration-150 cursor-pointer"
      ></div>
    </div>

    <div class="mt-4 flex gap-2 overflow-x-auto">
      <Button>
        <Component :size="16" />
        <p>Originais</p>
      </Button>
      <Button class="bg-purple-800 hover:bg-purple-950">
        <Joystick :size="16" />
        <p>Cassino</p>
      </Button>
      <Button class="bg-purple-800 hover:bg-purple-950">
        <Joystick :size="16" />
        <p>Slots</p>
      </Button>
      <Button class="bg-purple-800 hover:bg-purple-950">
        <Gamepad2 :size="16" />
        <p>Live Games</p>
      </Button>
      <Button class="bg-purple-800 hover:bg-purple-950">
        <Trophy :size="16" />
        <p>Sports</p>
      </Button>
    </div>

    <div class="mt-20">
      <div class="w-full h-[380px] bg-zinc-700 rounded-sm"></div>
    </div>
    <div class="mt-10">
      <div class="w-full h-[380px] bg-zinc-700 rounded-sm"></div>
    </div>
  </div>
</template>
