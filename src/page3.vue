<template lang="jade">
  f7-page(hide-bars-on-scroll='')
    f7-navbar(back-link='Back', title='Page 3', sliding='')
    f7-block This is page 3.
      br
      | Data-binding {{ mydata }}
      p.red This text is 
       span red
      p.cursive This is 
        span cursive
</template>

<script>
export default {
  name: 'page3',
  data () {
    return {
      mydata: 'this is mydata'
    }
  }
}
</script>

<style lang="sass?indentedSyntax">
  // Add your styles here.
  // See the following link for info on indented syntax:
  // http://sass-lang.com/documentation/file.INDENTED_SYNTAX.html

  .red
    span
      color: red

  .cursive
    span
      font-style: italic
</style>
