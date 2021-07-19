<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon roman-numeral4-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M12 7L14 17H16L18 7H16L15 12L14 7H12M11 7V9H10V15H11V17H7V15H8V9H7V7H11Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "RomanNumeral4Icon",
  props: {
    title: {
      type: String,
      default: "Roman Numeral4 icon"
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
