<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon language-kotlin-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M2 2H22L12 12L22 22H2Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "LanguageKotlinIcon",
  props: {
    title: {
      type: String,
      default: "Language Kotlin icon"
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
