<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon triforce-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M1.5,21L12,3.5L22.5,21H1.5M12,21L17,12H7L12,21Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "TriforceIcon",
  props: {
    title: {
      type: String,
      default: "Triforce icon"
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
