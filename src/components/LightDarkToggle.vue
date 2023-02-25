<script setup>
import IconMoon from "~icons/carbon/moon";
import IconSun from "~icons/carbon/sun";
import { useDark, useToggle } from "@vueuse/core";
const isDark = useDark();
const toggleDark = useToggle(isDark);
</script>

<template>
  <div v-auto-animate @click="toggleDark()">
    <div v-if="isDark">
      <icon-sun class="text-black dark:text-white" />
    </div>
    <div v-else><icon-moon class="text-black dark:text-white" /></div>
  </div>
</template>
