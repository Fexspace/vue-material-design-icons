<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon alpha-u-circle-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M9,7V15A2,2 0 0,0 11,17H13A2,2 0 0,0 15,15V7H13V15H11V7H9M12,2A10,10 0 0,1 22,12A10,10 0 0,1 12,22A10,10 0 0,1 2,12A10,10 0 0,1 12,2Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "AlphaUCircleIcon",
  props: {
    title: {
      type: String,
      default: "Alpha U Circle icon"
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
