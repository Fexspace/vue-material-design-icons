<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon text-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M21,6V8H3V6H21M3,18H12V16H3V18M3,13H21V11H3V13Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "TextIcon",
  props: {
    title: {
      type: String,
      default: "Text icon"
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
