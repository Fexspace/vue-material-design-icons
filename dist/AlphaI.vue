<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon alpha-i-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M14,7V9H13V15H14V17H10V15H11V9H10V7H14Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "AlphaIIcon",
  props: {
    title: {
      type: String,
      default: "Alpha I icon"
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
