<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon syllabary-katakana-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M4 4V6H18V6.09L14.29 9.79L15.71 11.21L20 6.91V4M11 9V13C11 15.78 10.25 16.89 8.36 18.46L9.64 20C11.75 18.24 13 16.22 13 13V9Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SyllabaryKatakanaIcon",
  props: {
    title: {
      type: String,
      default: "Syllabary Katakana icon"
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
