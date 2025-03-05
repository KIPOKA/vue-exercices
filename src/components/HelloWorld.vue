<template>
  <div
    :class="[
      'flex items-center justify-center h-screen',
      isDark ? 'bg-black' : 'bg-gray-100',
    ]"
  >
    <div class="text-center">
      <h1
        class="text-4xl font-bold"
        :class="isDark ? 'text-white' : 'text-blue-500'"
      >
        {{ msg || "Hello, Tailwind CSS with Vue!" }}
      </h1>
      <button
        @click="toggleTheme"
        class="mt-4 px-4 py-2 bg-blue-500 text-white rounded"
      >
        Toggle Theme
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      isDark: false,
    };
  },
  props: {
    msg: {
      type: String,
      default: "Hello, Tailwind CSS with Vue!",
    },
  },
  methods: {
    toggleTheme() {
      this.isDark = !this.isDark;
    },
  },
};
</script>
