<template>
  <ul class="at-menu__item-group">
    <li class="at-menu__item-group-title">
      <slot name="title"></slot>
      {{ title }}
    </li>
    <ul class="at-menu__item-group-list">
      <slot></slot>
    </ul>
  </ul>
</template>

<script>
export default {
  name: "AtMenuItemGroup",
  props: {
    title: {
      type: String,
      default: "",
    },
  },
};
</script>
