<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon home-import-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M15 13L11 9V12H2V14H11V17M22 12H20V21H4V16H6V19H18V11L12 5L7 10H4L12 2L22 12Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "HomeImportOutlineIcon",
  props: {
    title: {
      type: String,
      default: "Home Import Outline icon"
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
