<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon format-list-bulleted-triangle-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M5,15.5L7.5,20H2.5L5,15.5M9,19H21V17H9V19M5,9.5L7.5,14H2.5L5,9.5M9,13H21V11H9V13M5,3.5L7.5,8H2.5L5,3.5M9,7H21V5H9V7Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "FormatListBulletedTriangleIcon",
  props: {
    title: {
      type: String,
      default: "Format List Bulleted Triangle icon"
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
