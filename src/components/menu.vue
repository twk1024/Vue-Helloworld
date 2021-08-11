<template>
        <v-list-item>
          <v-list-item-content>
            <v-list-item-title class="title">
              {{ menutitle }}
            </v-list-item-title>
            <v-list-item-subtitle>
              {{ menusubtitle }}
            </v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
</template>

<script>
export default {
    props: ['menutitle', 'menusubtitle']
}
</script>
