<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon diving-scuba-flag-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M2,6L19,20H2V6M5,4L22,18V4H5Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "DivingScubaFlagIcon",
  props: {
    title: {
      type: String,
      default: "Diving Scuba Flag icon"
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
