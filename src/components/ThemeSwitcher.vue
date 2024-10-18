<template>
  <button @click="toggleDarkMode" class="border w-[200px] h-[50px] bg-amber-400">Theme</button>
</template>
<script>
export default {
  name: "ThemeSwitcher",
  data() {
    return {
      darkMode: false,
    };
  },
  mounted() {
    if (localStorage.getItem("theme") === "dark") {
      this.darkMode = true;
      document.documentElement.classList.add("dark");
    }
  },
  methods: {
    toggleDarkMode() {
      this.darkMode = !this.darkMode;
      if (this.darkMode) {
        document.documentElement.classList.add("dark");
        localStorage.setItem("theme", "dark");
      } else {
        document.documentElement.classList.remove("dark");
        localStorage.setItem("theme", "light");
      }
    },
  },
};
</script>
