<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon alpha-g-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M11,7A2,2 0 0,0 9,9V15A2,2 0 0,0 11,17H13A2,2 0 0,0 15,15V11H13V15H11V9H15V7H11Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "AlphaGIcon",
  props: {
    title: {
      type: String,
      default: "Alpha G icon"
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
