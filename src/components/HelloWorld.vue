<template>
  <div :class="['flex items-center justify-center h-screen', randomBgColor]">
    <h1 class="text-4xl font-bold text-yellow-500">
      {{ msg || "Hello, Tailwind CSS with Vue!" }}
    </h1>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      bgColors: [
        "bg-red-200",
        "bg-blue-200",
        "bg-green-200",
        "bg-purple-200",
        "bg-yellow-200",
      ],
      randomBgColor: "",
    };
  },
  props: {
    msg: {
      type: String,
      default: "Hello, Tailwind CSS with Vue!",
    },
  },
  created() {
    this.randomBgColor =
      this.bgColors[Math.floor(Math.random() * this.bgColors.length)];
  },
};
</script>
