<script setup lang="ts">
// Need to access the defineProps returned value to
// infer types although you never use the props directly
import { Button } from "ant-design-vue";
const props = defineProps<{
  color: "blue" | "red";
}>();
</script>

<template>
  <div>{{ color }}</div>

  <!-- 注释Button组件后，可以生成helloworld的声明文件 -->
  <Button>test</Button>
</template>

