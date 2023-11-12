<script setup>
defineProps({
  event: {
    type: Object,
    required: true
  }
})
</script>

<template>
  <div class="container mx-auto text-black">
    <div class="text-base text-center">
      <div class="border w-96 py-9 mx-auto border-black">
        This is the <span class="font-bold">{{ event.title }}</span>
        <br />
        on
        <span class="font-bold"
          >{{ event.date }} at {{ event.location }} start from {{ event.time }}</span
        >
      </div>
    </div>
  </div>
</template>

<style scoped></style>
