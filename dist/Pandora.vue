<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon pandora-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M10,20A1,1 0 0,1 9,21H4V3H13.71A6.75,6.75 0 0,1 20.46,9.75C20.46,13.5 17.44,16.5 13.71,16.5H10V20Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "PandoraIcon",
  props: {
    title: {
      type: String,
      default: "Pandora icon"
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
