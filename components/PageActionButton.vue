<template>
  <a class="inline-flex items-center bg-transparent border border-gray-400 rounded text-xs" href="#">
    <div class="flex px-2 py-1 border-r border-gray-400 rounded-l">
      <slot></slot>
      <span class="ml-1">{{ text }}</span>
    </div>
    <span class="px-2 py-1 bg-white rounded-r font-bold">{{ number }}</span>
  </a>
</template>

<script>
export default {
  props: ['text', 'number'],
}
</script>
