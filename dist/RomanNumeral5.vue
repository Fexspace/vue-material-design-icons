<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon roman-numeral5-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M9 7L11 17H13L15 7H13L12 12L11 7H9Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "RomanNumeral5Icon",
  props: {
    title: {
      type: String,
      default: "Roman Numeral5 icon"
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
