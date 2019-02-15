<template>
  <div class="about">
    <h1>Hello {{ their_name }}, this is an about page</h1>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna ali...</p>
  </div>
</template>

<script>
export default {
  name: 'About',
  data() {
    return {
        /* Funkar inte av n�gon anledning, vid "falskt" returneras inte 'Hi' */
      their_name: this.$route.params.name != '' ? 'true' : 'Hi'
    }
  }
}
</script>