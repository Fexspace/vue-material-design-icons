<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon view-module-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M4 5V18H21V5H4M14 7V10.5H11V7H14M6 7H9V10.5H6V7M6 16V12.5H9V16H6M11 16V12.5H14V16H11M19 16H16V12.5H19V16M16 10.5V7H19V10.5H16Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "ViewModuleOutlineIcon",
  props: {
    title: {
      type: String,
      default: "View Module Outline icon"
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
