<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon comma-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M7,3H16.95V12.96L12.96,20.94H8L11.97,12.96H7V3Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "CommaIcon",
  props: {
    title: {
      type: String,
      default: "Comma icon"
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
