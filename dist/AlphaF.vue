<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon alpha-f-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M9,7V17H11V13H14V11H11V9H15V7H9Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "AlphaFIcon",
  props: {
    title: {
      type: String,
      default: "Alpha F icon"
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
