<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon transfer-down-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M16,3V5H8V3H16M16,7V9H8V7H16M16,11V13H8V11H16M5,15H19L12,22L5,15Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "TransferDownIcon",
  props: {
    title: {
      type: String,
      default: "Transfer Down icon"
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
