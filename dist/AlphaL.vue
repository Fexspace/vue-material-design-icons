<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon alpha-l-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M9,7V17H15V15H11V7H9Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "AlphaLIcon",
  props: {
    title: {
      type: String,
      default: "Alpha L icon"
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
