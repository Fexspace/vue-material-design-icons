<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon home-floor-l-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M12,3L2,12H5V20H19V12H22L12,3M9,8H11V16H15V18H9V8Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "HomeFloorLIcon",
  props: {
    title: {
      type: String,
      default: "Home Floor L icon"
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
