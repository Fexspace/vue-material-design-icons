<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon post-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M3 3V21H21V3H3M18 18H6V17H18V18M18 16H6V15H18V16M18 12H6V6H18V12Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "PostIcon",
  props: {
    title: {
      type: String,
      default: "Post icon"
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
