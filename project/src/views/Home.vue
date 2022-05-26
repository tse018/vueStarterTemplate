<template>
   <Grid />
</template>

<script>
import Grid from '../components/Grid.vue';

import seoMixin from '../mixins/seoMixin.js';

export default {
   mixins: [seoMixin],

   components: {
      Grid,
   },

   created() {
      this.metaTags({
         title: 'Vue Starter Template',
		});
   }
}
</script>

<style>
</style>
