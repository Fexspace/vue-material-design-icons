<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon bookmark-multiple-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M9,1H19A2,2 0 0,1 21,3V19L19,18.13V3H7A2,2 0 0,1 9,1M15,20V7H5V20L10,17.82L15,20M15,5C16.11,5 17,5.9 17,7V23L10,20L3,23V7A2,2 0 0,1 5,5H15Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "BookmarkMultipleOutlineIcon",
  props: {
    title: {
      type: String,
      default: "Bookmark Multiple Outline icon"
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
