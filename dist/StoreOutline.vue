<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon store-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M18.36 9L18.96 12H5.04L5.64 9H18.36M20 4H4V6H20V4M20 7H4L3 12V14H4V20H14V14H18V20H20V14H21V12L20 7M6 18V14H12V18H6Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "StoreOutlineIcon",
  props: {
    title: {
      type: String,
      default: "Store Outline icon"
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
