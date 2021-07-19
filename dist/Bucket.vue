<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon bucket-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M3 4H21V7H20L17.5 21H6.5L4 7H3V4Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "BucketIcon",
  props: {
    title: {
      type: String,
      default: "Bucket icon"
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
