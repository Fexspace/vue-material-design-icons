<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon delta-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M12,7.77L18.39,18H5.61L12,7.77M12,4L2,20H22">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "DeltaIcon",
  props: {
    title: {
      type: String,
      default: "Delta icon"
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
