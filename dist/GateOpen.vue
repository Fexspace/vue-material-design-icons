<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon gate-open-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M7 20V6H5V10H3V8H1V20H3V18H5V20H7M3 16V12H5V16H3M21 8V10H19V6H17V20H19V18H21V20H23V8H21M21 16H19V12H21V16Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "GateOpenIcon",
  props: {
    title: {
      type: String,
      default: "Gate Open icon"
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
