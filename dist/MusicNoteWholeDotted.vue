<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon music-note-whole-dotted-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M10 15A2 2 0 1 1 8 17A2 2 0 0 1 10 15M10 13A4 4 0 1 0 14 17A4 4 0 0 0 10 13M16.5 17A1.5 1.5 0 1 1 15 18.5A1.5 1.5 0 0 1 16.5 17Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "MusicNoteWholeDottedIcon",
  props: {
    title: {
      type: String,
      default: "Music Note Whole Dotted icon"
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
