<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon music-note-half-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M16 3H14V13.56A3.96 3.96 0 0 0 12 13A4 4 0 1 0 16 17V3M12 19A2 2 0 1 1 14 17A2 2 0 0 1 12 19Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "MusicNoteHalfIcon",
  props: {
    title: {
      type: String,
      default: "Music Note Half icon"
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
