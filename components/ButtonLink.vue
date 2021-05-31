<template>
  <a class="border rounded p-2" :href="link">
    <slot></slot>
  </a>
</template>

<script>
export default {
  props: {
    link: {
      type: String,
      default: '#',
      nullable: true,
    }
  },
}
</script>
