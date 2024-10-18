<template>
    <AppHeader />
    <ThemeSwitcher />
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import ThemeSwitcher from "./components/ThemeSwitcher.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    ThemeSwitcher,
  },
  data() {
    return {
    };
  },
};
</script>
