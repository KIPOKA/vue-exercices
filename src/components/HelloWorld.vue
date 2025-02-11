<template>
  <div
    class="flex items-center justify-center h-screen bg-cover bg-center"
    style="background-image: url('https://via.placeholder.com/150')"
  >
    <h1 class="text-4xl font-bold text-white">Hello, Tailwind CSS with Vue!</h1>
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
