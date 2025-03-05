<template>
  <div class="flex items-center justify-center h-screen bg-gray-100">
    <h1 class="text-4xl font-bold text-indigo-500">
      {{ displayedText }}
    </h1>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      fullText: "Hello, Tailwind CSS with Vue!",
      displayedText: "",
      index: 0,
    };
  },
  mounted() {
    this.typewriterEffect();
  },
  methods: {
    typewriterEffect() {
      const interval = setInterval(() => {
        if (this.index < this.fullText.length) {
          this.displayedText += this.fullText[this.index];
          this.index++;
        } else {
          clearInterval(interval);
        }
      }, 100);
    },
  },
};
</script>
