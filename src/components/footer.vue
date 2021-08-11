<template>
    <v-footer color="primary" dark>
      <v-spacer/>{{ footer }}
    </v-footer>
</template>

<script>
export default {
    props: ['footer']
}
</script>
