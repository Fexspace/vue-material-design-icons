<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon volume-low-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M7,9V15H11L16,20V4L11,9H7Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "VolumeLowIcon",
  props: {
    title: {
      type: String,
      default: "Volume Low icon"
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
