<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon octagon-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M15.73,3H8.27L3,8.27V15.73L8.27,21H15.73L21,15.73V8.27">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "OctagonIcon",
  props: {
    title: {
      type: String,
      default: "Octagon icon"
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
