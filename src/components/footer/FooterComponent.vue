<template>
    <v-footer
      dark>
      <v-row
        justify="center"
        class="my-4 text-center" >
        <v-col cols="12">
          <v-btn variant="plain" :href=link.url v-for="link in links" :key="link">{{ link.name }}</v-btn>
        </v-col>
        <v-col>&copy; 2024 Tweetie</v-col>
      </v-row>
    </v-footer>
</template>
<script>
export default {
  data: () => {
    return { links: [
      {
        name:'Home', url:'/'
      },
      {
        name:'About', url:'/'
      },
      {
        name:'Admin', url:'/admin'
      },
    ] };
  },
};
</script>