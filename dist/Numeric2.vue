<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon numeric2-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M9,7V9H13V11H11A2,2 0 0,0 9,13V17H11L15,17V15H11V13H13A2,2 0 0,0 15,11V9A2,2 0 0,0 13,7H9Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "Numeric2Icon",
  props: {
    title: {
      type: String,
      default: "Numeric2 icon"
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
