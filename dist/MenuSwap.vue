<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon menu-swap-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M12,6L7,11H17L12,6M7,13L12,18L17,13H7Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "MenuSwapIcon",
  props: {
    title: {
      type: String,
      default: "Menu Swap icon"
    },
    decorative: {
      type: Boolean,
      default: false
    },
    fillColor: {
      type: String,
      default: "currentColor"
    },
    size: {
      type: Number,
      default: 24
    }
  }
}
</script>
