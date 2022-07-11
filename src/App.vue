<script setup lang="ts">
import Position from './Position.vue';
import { PositionList } from './Position.ts';
</script>

<template>
  <Position :position="PositionList.First" />
</template>
