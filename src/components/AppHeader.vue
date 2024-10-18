<template>
  <header>
    <div class="flex bg-slate-400 w-100% h-[65px] justify-between items-center">
      <div class="logo">
        <div class="pl-10">
          <a href="#">
            <img
              class="w-[50px] h-[50px]"
              src="../assets/logo.svg"
              alt="application logo"
            />
          </a>
        </div>
      </div>
      <nav class="flex gap-3 pr-10">
        <ul
          v-for="(link, index) in headerLinks"
          :key="index"
        >
          <li>
            <a class="" :href="link.url">{{ link.name }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>
<script>
import { HeaderLinks } from "@/constants/const.ts";

export default {
  name: "AppHeader",
  data() {
    return {
      headerLinks: HeaderLinks,
    };
  },
};
</script>
