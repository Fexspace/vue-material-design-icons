<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon relation-one-or-many-to-only-one-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M22 15V17H21V19H19V17H18V19H16V17H11V9H7V11H5V9L3 11H2V5H3L5 7V5H7V7H13V15H16V13H18V15H19V13H21V15Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "RelationOneOrManyToOnlyOneIcon",
  props: {
    title: {
      type: String,
      default: "Relation One Or Many To Only One icon"
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
