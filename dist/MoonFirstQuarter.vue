<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon moon-first-quarter-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M12 2V22A10 10 0 0 0 12 2Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "MoonFirstQuarterIcon",
  props: {
    title: {
      type: String,
      default: "Moon First Quarter icon"
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
