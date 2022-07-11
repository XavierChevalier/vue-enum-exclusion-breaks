<script setup lang="ts">
import { PositionList } from './Position.ts';

type FirstAndSecond = Exclude<PositionList, PositionList.Third>;

defineProps<{
  position: FirstAndSecond; // [Vue warn]: Invalid prop: type check failed for prop "position". Expected Object, got String with value "FIRST".
}>();
</script>

<template>
  <h1>{{ position }}</h1>
</template>
