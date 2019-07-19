<template>
  <div id="welcome-section" class="welcome-section">
    <h1>Hello! :)</h1>
    <h1>My name's {{ authorName }}</h1>
    <p>a Front End Developer</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      authorName: 'Muhammad'
    }
  }
}
</script>

<style></style>
