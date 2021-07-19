<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon note-minus-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M16 3H4C2.89 3 2 3.89 2 5V19C2 20.1 2.89 21 4 21H20C21.11 21 22 20.11 22 19V9L16 3M20 19H4V5H13V12H20V19M15 10V4.5L20.5 10H15M6 13H12V15H6V13Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "NoteMinusOutlineIcon",
  props: {
    title: {
      type: String,
      default: "Note Minus Outline icon"
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
