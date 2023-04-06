<template>
  <button
    :type="type"
    :class="bgClass"
    class="
      px-6
      py-2
      font-semibold
      text-white
      rounded-md
      hover:opacity-95
      focus:outline-none">
    <slot />
  </button>
</template>

<script>
export default {
  name: 'KButton',
  props: {
    type: {
      type: String,
      default: 'save',
    },
    bgClass: {
      type: String,
      default: 'bg-blue-500',
    },
  },
};
</script>