<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon relation-one-to-one-or-many-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M22 13V19H21L19 17V19H17V17H11V9H7V11H5V9H2V7H5V5H7V7H13V15H17V13H19V15L21 13Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "RelationOneToOneOrManyIcon",
  props: {
    title: {
      type: String,
      default: "Relation One To One Or Many icon"
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
