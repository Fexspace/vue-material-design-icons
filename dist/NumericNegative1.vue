<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon numeric-negative1-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M13 7V9H15V17H17V7H13M11 13H5V11H11V13Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "NumericNegative1Icon",
  props: {
    title: {
      type: String,
      default: "Numeric Negative1 icon"
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
