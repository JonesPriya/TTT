<template lang="pug">
.c-details
  .details
    .name
      label Your Name*: 
      input(type="text", name="firstname", value=" ") 
    .mail
      label Email Address*: 
      input(type="text", name="firstname", value=" ") 
    .message
        label Message*: 
        input(type="text", name="firstname", value=" ") 
    .cta
      a.btn.btn-primary
        nuxt-link(to="") Get Started
  .contact-us
    .c-details
      p Bangalore,India
      span hello@targetthoughts.com | 98765 43219
  
</template>

<script>
export default {
  
}
</script>

<style lang="sass" scoped>
@import 'assets/styles/includes'

.c-details
  @include flex(stretch)
  min-height: 100vh
  @media (max-width: $br-desktop-small)
    display: block
  .details
    margin: $s*2 0
    height: 40rem
    width: 32rem
    text-align: center
    @media (max-width: $br-desktop-small)
      height: auto
      margin: $s 0
    .name,
    .mail,
    .message,
    .cta
      margin: $s*2 0

  .contact-us
    width: 40%
    @include flex(center, center)
    @media (max-width: $br-desktop-small)
      width: 100%
      padding-top: $s*10
</style>


