<script lang="ts">
export default {
  name: "Button",
  props: {
    disabled: Boolean,
    class: String,
  },
};
</script>

<template>
  <button
    :class="class"
    :disabled="disabled"
    class="px-4 py-2 rounded-lg font-semibold border bg-purple-600 border-purple-800 hover:bg-purple-800 ease-in-out duration-300"
  >
    <div class="flex gap-2 text-white items-center">
      <slot></slot>
    </div>
  </button>
</template>
