<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon view-sequential-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M3 5H21V9H3V5M3 10H21V14H3V10M3 15H21V19H3V15Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "ViewSequentialIcon",
  props: {
    title: {
      type: String,
      default: "View Sequential icon"
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
