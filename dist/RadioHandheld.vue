<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon radio-handheld-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M9,2A1,1 0 0,0 8,3C8,8.67 8,14.33 8,20C8,21.11 8.89,22 10,22H15C16.11,22 17,21.11 17,20V9C17,7.89 16.11,7 15,7H10V3A1,1 0 0,0 9,2M10,9H15V13H10V9Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "RadioHandheldIcon",
  props: {
    title: {
      type: String,
      default: "Radio Handheld icon"
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
