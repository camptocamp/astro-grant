<script setup lang="ts">
const props = defineProps<{
  href?: string
  title?: string
}>()
</script>

<template>
    <a :href="props.href" :title="props.title" class="inline-flex items-center font-medium text-blue-600 dark:text-blue-500 hover:underline">
        <slot>A link...</slot>
        <svg aria-hidden="true" class="w-5 h-5 ml-1" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M12.293 5.293a1 1 0 011.414 0l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-2.293-2.293a1 1 0 010-1.414z" clip-rule="evenodd"></path></svg>
    </a>
</template>