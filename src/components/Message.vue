<script>
export default {
  props: {
    active: Boolean,
    default: false,
  },
}
</script>

<template>
  <article
    class="message"
    :class="{ 'message--hidden': !active }"
  >
    <div class="message-header">
      <slot name="header"></slot>
      <button class="delete"></button>
    </div>

    <div class="message-body">
      Something went wrong
    </div>
  </article>
</template>

<style></style>