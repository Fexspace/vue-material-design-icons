<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon view-agenda-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M21 13H3A1 1 0 0 0 2 14V20A1 1 0 0 0 3 21H21A1 1 0 0 0 22 20V14A1 1 0 0 0 21 13M20 19H4V15H20M21 3H3A1 1 0 0 0 2 4V10A1 1 0 0 0 3 11H21A1 1 0 0 0 22 10V4A1 1 0 0 0 21 3M20 9H4V5H20Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "ViewAgendaOutlineIcon",
  props: {
    title: {
      type: String,
      default: "View Agenda Outline icon"
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
