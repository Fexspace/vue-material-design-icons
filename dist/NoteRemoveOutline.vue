<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon note-remove-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M16 3H4C2.89 3 2 3.89 2 5V19C2 20.1 2.89 21 4 21H20C21.11 21 22 20.11 22 19V9L16 3M20 19H4V5H13V12H20V19M15 10V4.5L20.5 10H15M11.83 12.59L10.41 14L11.83 15.41L10.41 16.83L9 15.41L7.59 16.83L6.17 15.41L7.59 14L6.17 12.59L7.59 11.17L9 12.59L10.41 11.17L11.83 12.59Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "NoteRemoveOutlineIcon",
  props: {
    title: {
      type: String,
      default: "Note Remove Outline icon"
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
