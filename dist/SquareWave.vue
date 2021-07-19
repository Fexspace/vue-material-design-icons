<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon square-wave-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M2 2V12H4V4H11V22H22V12H20V20H13V2H2Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SquareWaveIcon",
  props: {
    title: {
      type: String,
      default: "Square Wave icon"
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
