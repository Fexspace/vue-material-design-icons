<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon navigation-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M12 7.3L16.3 17.7L12.8 16.2L12 15.8L11.2 16.2L7.7 17.7L12 7.3M12 2L4.5 20.3L5.2 21L12 18L18.8 21L19.5 20.3L12 2Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "NavigationOutlineIcon",
  props: {
    title: {
      type: String,
      default: "Navigation Outline icon"
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
