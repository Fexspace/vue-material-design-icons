<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon music-note-whole-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M12 15A2 2 0 1 1 10 17A2 2 0 0 1 12 15M12 13A4 4 0 1 0 16 17A4 4 0 0 0 12 13Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "MusicNoteWholeIcon",
  props: {
    title: {
      type: String,
      default: "Music Note Whole icon"
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
