<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon align-horizontal-right-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M18 13V19H2V13H18M8 5V11H18V5H8M20 2V22H22V2H20Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "AlignHorizontalRightIcon",
  props: {
    title: {
      type: String,
      default: "Align Horizontal Right icon"
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
