<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon seat-individual-suite-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M7,13A3,3 0 0,0 10,10A3,3 0 0,0 7,7A3,3 0 0,0 4,10A3,3 0 0,0 7,13M19,7H11V14H3V7H1V17H23V11A4,4 0 0,0 19,7Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SeatIndividualSuiteIcon",
  props: {
    title: {
      type: String,
      default: "Seat Individual Suite icon"
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
