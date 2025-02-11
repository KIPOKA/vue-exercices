<template>
  <div class="flex items-center justify-center h-screen bg-gray-100">
    <h1 class="text-4xl font-bold text-red-600">
      Hello, Tailwind CSS with Vue!
    </h1>
    <button class="mt-4 px-6 py-2 bg-green-500 text-white rounded">
      Click Me
    </button>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>
