<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon format-quote-open-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M11 18V10H9.12L11.12 6H5.38L3 10.76V18M9 16H5V11.24L6.62 8H7.88L5.88 12H9M21 18V10H19.12L21.12 6H15.38L13 10.76V18M19 16H15V11.24L16.62 8H17.88L15.88 12H19Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "FormatQuoteOpenOutlineIcon",
  props: {
    title: {
      type: String,
      default: "Format Quote Open Outline icon"
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
