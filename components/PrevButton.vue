<template>
  <button
    @click="onClick"
    class="
      rounded-full
      text-white
      w-[113px]
      h-[50px]
      bg-green
      relative
      py-2
      px-2
      hover:bg-receipt
      focus:outline-none focus:ring-2 focus:ring-green-600 focus:ring-opacity-50
    "
  >
    <div class="flex flex-wrap items-center">
      <svg
        width="33"
        height="33"
        viewBox="0 0 33 33"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <rect width="33" height="33" rx="16.5" fill="white" />
        <path
          d="M9.0257 15.8218L18.4693 7.28048C18.8837 6.90651 19.555 6.90651 19.9705 7.28048C20.3848 7.65444 20.3848 8.26186 19.9705 8.63583L11.2759 16.4995L19.9694 24.3631C20.3838 24.7371 20.3838 25.3445 19.9694 25.7194C19.555 26.0934 18.8826 26.0934 18.4683 25.7194L9.02465 17.1781C8.61655 16.808 8.61655 16.191 9.0257 15.8218Z"
          fill="#8BAC3E"
        />
      </svg>
      <span class="mx-2 my-1 font-medium text-base text-justify">PREV</span>
    </div>
  </button>
</template>
<script>
export default {
  name: 'PrevButton',
  props: {
    onClick: {
      type: Function,
      default: () => null,
      required: true,
    },
  },
}
</script>