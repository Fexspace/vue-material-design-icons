<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon align-horizontal-left-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M22 13V19H6V13H22M6 5V11H16V5H6M2 2V22H4V2H2">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "AlignHorizontalLeftIcon",
  props: {
    title: {
      type: String,
      default: "Align Horizontal Left icon"
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
