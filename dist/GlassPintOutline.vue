<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon glass-pint-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M4 2L6 22H17L19 2H4M6.2 4H16.8L15.2 20H7.8L6.2 4Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "GlassPintOutlineIcon",
  props: {
    title: {
      type: String,
      default: "Glass Pint Outline icon"
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
