<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon sign-pole-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M11 3L12 2L13 3V20C14.11 20 15 20.9 15 22H9C9 20.9 9.9 20 11 20V3Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SignPoleIcon",
  props: {
    title: {
      type: String,
      default: "Sign Pole icon"
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
