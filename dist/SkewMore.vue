<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon skew-more-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M12.5,11L10.41,20H5.5L7.59,11H12.5M15,9H6L3,22H12L15,9M21,6L17,2V5H9V7H17V10L21,6Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SkewMoreIcon",
  props: {
    title: {
      type: String,
      default: "Skew More icon"
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
