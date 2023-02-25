<script setup>
import IconSearch from "~icons/carbon/search";
import CountryCard from '../components/CountryCard.vue'
</script>

<template>
  <div class="h-full max-h-full flex flex-col">
    <div class="flex flex-row justify-between flex-none my-8">
      <div
        class="_searchBar bg-[#2b3743] rounded p-2 flex flex-row items-center dark:text-white"
      >
        <icon-search class="mx-2" />
        <input type="text" placeholder="Search for a country" class="bg-[#2b3743] border-none outline-none" />
      </div>

      <select
        name="cars"
        id="cars"
        class="bg-[#2b3743] rounded p-2 px-4 flex flex-row items-center dark:text-white"
      >
        <option disabled selected value>Filter by Region</option>
        <option value="volvo">Volvo</option>
        <option value="saab">Saab</option>
        <option value="opel">Opel</option>
        <option value="audi">Audi</option>
      </select>
    </div>
    <div v-auto-animate class="_countries  dark:text-white flex-1 flex flex-row flex-wrap gap-12 justify-between overflow-y-auto">
      <CountryCard />
      <CountryCard />
      <CountryCard />
      <CountryCard />
      <CountryCard />
      <CountryCard />
      <CountryCard />
      <CountryCard />
    </div>
  </div>
</template>
