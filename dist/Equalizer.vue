<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon equalizer-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M10,20H14V4H10V20M4,20H8V12H4V20M16,9V20H20V9H16Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "EqualizerIcon",
  props: {
    title: {
      type: String,
      default: "Equalizer icon"
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
