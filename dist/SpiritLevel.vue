<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon spirit-level-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M22 8H2V16H22V8M18 14V10H20V14H18M11 12H13C14.1 12 15 11.11 15 10H17V14H7V10H9C9 11.11 9.9 12 11 12M4 14V10H6V14H4Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SpiritLevelIcon",
  props: {
    title: {
      type: String,
      default: "Spirit Level icon"
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
