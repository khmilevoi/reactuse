<script setup lang="ts">
const props = defineProps<{
  hook: string;
}>();

const repositoryLink = `https://github.com/siberiacancode/reactuse/blob/main/packages/core/src/hooks/${props.hook}`;

const sourceLink = `${repositoryLink}/${props.hook}.ts`;
const demoLink = `${repositoryLink}/${props.hook}.demo.tsx`;
</script>

<template>
  <a target="_blank" :href="sourceLink">Source</a> •
  <a target="_blank" :href="demoLink">Demo</a>
</template>
