<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon arrow-left-right-bold-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M8,14V18L2,12L8,6V10H16V6L22,12L16,18V14H8Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "ArrowLeftRightBoldIcon",
  props: {
    title: {
      type: String,
      default: "Arrow Left Right Bold icon"
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
