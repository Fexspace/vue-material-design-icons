<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon test-tube-empty-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M7,2H17V4H16V18A4,4 0 0,1 12,22A4,4 0 0,1 8,18V4H7V2M14,4H10V18A2,2 0 0,0 12,20A2,2 0 0,0 14,18V4Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "TestTubeEmptyIcon",
  props: {
    title: {
      type: String,
      default: "Test Tube Empty icon"
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
