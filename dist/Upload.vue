<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon upload-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M9,16V10H5L12,3L19,10H15V16H9M5,20V18H19V20H5Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "UploadIcon",
  props: {
    title: {
      type: String,
      default: "Upload icon"
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
