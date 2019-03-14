<template lang="pug">
section.c-details
  .container
    .details
      .name
        label Your Name *: 
        input(type="text", name="firstname", value=" ") 
      .mail
        label Email Address *: 
        input(type="text", name="firstname", value=" ") 
      .message
          label Message *: 
          input(type="text", name="firstname", value=" ") 
      .cta
        a.btn.btn-primary
          nuxt-link(to="") Submit
    .contact-us
      .c-details
        p Bangalore,India
        p hello@targetthoughts.com 
        p 98765 43219
  
</template>

<script>
export default {
  
}
</script>

<style lang="sass" scoped>
@import 'assets/styles/includes'

section.c-details
  .container
    @include flex(stretch)
    @media (max-width: $br-desktop-small)
      display: block
    .details
      margin: $s*2 0
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
      @media (max-width: $br-desktop-small)
        width: 100%
        padding-top: $s*10
      .c-details
        display: block
        p
          font-size: 1rem
</style>


