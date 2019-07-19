<template>
  <p>{{formattedMessage}}</p>
</template>

<script>
export default {
  name: "SecretComponent",
  props: {
    message: String
  },
  computed: {
    formattedMessage() {
      return this.message.substring(0, this.message.length - 3) + "*".repeat(3);
    }
  }
};
</script>

<style></style>