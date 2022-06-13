<script setup lang="ts">
import CharacterSheet from "@/components/CharacterSheet.vue";
import Spells from "@/components/Spells.vue";

const character = {
  alignment: "Chaotic Good",
  name: "Wilhelm Helldoom Bloodlord",
  occupation: "Paladin",
  level: "4",
  race: "Goblin",
};
</script>

<template>
  <div id="app">
    <CharacterSheet :character="character" />
    <Spells />
  </div>
</template>

<style>
@import "./assets/base.css";
@import "./assets/utilities.css";
</style>
