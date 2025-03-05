<template>
  <div
    class="flex items-center justify-center h-screen bg-gray-100 dark:bg-gray-800"
  >
    <h1 class="text-4xl font-bold text-purple-500 dark:text-yellow-300">
      {{ msg || "Hello, Tailwind CSS with Vue!" }}
    </h1>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: {
      type: String,
      default: "Hello, Tailwind CSS with Vue!",
    },
  },
};
</script>
