<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon moon-full-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M12 2A10 10 0 1 1 2 12A10 10 0 0 1 12 2Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "MoonFullIcon",
  props: {
    title: {
      type: String,
      default: "Moon Full icon"
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
