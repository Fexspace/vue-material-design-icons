<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon home-floor-negative1-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M12,3L2,12H5V20H19V12H22L12,3M11,15H7V13H11V15M15,18H13V10H11V8H15V18Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "HomeFloorNegative1Icon",
  props: {
    title: {
      type: String,
      default: "Home Floor Negative1 icon"
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
