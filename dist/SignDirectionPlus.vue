<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon sign-direction-plus-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M13 20H13.09A5.5 5.5 0 0 0 13.81 22H9A2 2 0 0 1 11 20V12H3.5L6 9.5L3.5 7H11V3L12 2L13 3V7H18L20.5 9.5L18 12H13M18 15V18H15V20H18V23H20V20H23V18H20V15Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SignDirectionPlusIcon",
  props: {
    title: {
      type: String,
      default: "Sign Direction Plus icon"
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
