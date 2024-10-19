<template>
    <AppHeader />
    <ThemeSwitcher />
    <AppCard />
</template>

<script>
import AppCard from "./components/AppCard.vue";
import AppHeader from "./components/AppHeader.vue";
import ThemeSwitcher from "./components/ThemeSwitcher.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    ThemeSwitcher,
    AppCard,
  },
  data() {
    return {
    };
  },
};
</script>
