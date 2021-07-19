<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon network-strength1-alert-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M21 1L1 21H17V19H11V13.8L19 5.8V9H21M19 11V17H21V11M19 19V21H21V19">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "NetworkStrength1AlertIcon",
  props: {
    title: {
      type: String,
      default: "Network Strength1 Alert icon"
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
