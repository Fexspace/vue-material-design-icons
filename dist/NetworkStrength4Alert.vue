<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon network-strength4-alert-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M19 17H21V11H19M19 21H21V19H19M1 21H17V9H21V1">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "NetworkStrength4AlertIcon",
  props: {
    title: {
      type: String,
      default: "Network Strength4 Alert icon"
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
