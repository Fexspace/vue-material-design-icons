<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon transfer-up-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M8,21V19H16V21H8M8,17V15H16V17H8M8,13V11H16V13H8M19,9H5L12,2L19,9Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "TransferUpIcon",
  props: {
    title: {
      type: String,
      default: "Transfer Up icon"
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
