<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon message-minus-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M20 2C21.11 2 22 2.9 22 4V16C22 17.11 21.11 18 20 18H6L2 22V4C2 2.89 2.9 2 4 2H20M8 9V11H16V9H8Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "MessageMinusIcon",
  props: {
    title: {
      type: String,
      default: "Message Minus icon"
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
