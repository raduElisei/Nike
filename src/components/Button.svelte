<script>
  export let iconURL = "";
</script>

<button
  class="flex justify-center items-center gap-2 px-7 py-4 border font-montserrat text-lg leading-none bg-coral-red rounded-full text-white border-coral-red"
>
  <slot>Click Me</slot>
  {#if iconURL}
    <img
      src={iconURL}
      alt="arrow right icon"
      class="ml-2 rounded-full w-5 h-5"
    />
  {/if}
</button>
