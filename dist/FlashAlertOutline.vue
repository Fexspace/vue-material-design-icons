<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon flash-alert-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M5,2H15L11.5,9H15L8,22V14H5V2M7,4V12H10V14.66L12,11H8.24L11.76,4M17,15H19V17H17V15M17,7H19V13H17V7Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "FlashAlertOutlineIcon",
  props: {
    title: {
      type: String,
      default: "Flash Alert Outline icon"
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
