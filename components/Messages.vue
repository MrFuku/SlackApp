<template>
  <div class="chats-container">
    <Message v-for="message in messages" :message="message" />
  </div>
</template>

<script>
import Message from '~/components/Message'

export default {
  components: {
    Message
  },
  props: ['messages'],
}
</script>

<style scoped>
.chats-container {
  padding: 16px;
}

</style>
