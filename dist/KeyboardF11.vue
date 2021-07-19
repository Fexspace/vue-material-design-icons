<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon keyboard-f11-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M3 7H9V9H5V11H8V13H5V17H3V7M11 7H15V17H13V9H11V7M17 7H21V17H19V9H17V7Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "KeyboardF11Icon",
  props: {
    title: {
      type: String,
      default: "Keyboard F11 icon"
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
