<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon car-battery-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M4,3V6H1V20H23V6H20V3H14V6H10V3H4M3,8H21V18H3V8M15,10V12H13V14H15V16H17V14H19V12H17V10H15M5,12V14H11V12H5Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "CarBatteryIcon",
  props: {
    title: {
      type: String,
      default: "Car Battery icon"
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
