<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon keyboard-caps-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M6,18H18V16H6M12,8.41L16.59,13L18,11.58L12,5.58L6,11.58L7.41,13L12,8.41Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "KeyboardCapsIcon",
  props: {
    title: {
      type: String,
      default: "Keyboard Caps icon"
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
