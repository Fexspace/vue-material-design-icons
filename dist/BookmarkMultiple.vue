<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon bookmark-multiple-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M15,5A2,2 0 0,1 17,7V23L10,20L3,23V7C3,5.89 3.9,5 5,5H15M9,1H19A2,2 0 0,1 21,3V19L19,18.13V3H7A2,2 0 0,1 9,1Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "BookmarkMultipleIcon",
  props: {
    title: {
      type: String,
      default: "Bookmark Multiple icon"
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
