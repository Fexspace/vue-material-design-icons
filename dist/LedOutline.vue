<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon led-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M12,6A4,4 0 0,0 8,10V16H6V18H9V23H11V18H13V23H15V18H18V16H16V10A4,4 0 0,0 12,6M12,8A2,2 0 0,1 14,10V15H10V10A2,2 0 0,1 12,8Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "LedOutlineIcon",
  props: {
    title: {
      type: String,
      default: "Led Outline icon"
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
