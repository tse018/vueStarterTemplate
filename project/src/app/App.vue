<template>
   <Header />
   <RouterView />
   <Footer />
</template>

<script>
import Header from '../components/Header.vue';
import Footer from '../components/Footer.vue';

import seoMixin from '../mixins/seoMixin.js';

export default {
   mixins: [seoMixin],
   
   components: {
      Header,
      Footer
   },

   async created() {
      this.metaTags({
         title: 'Vue Starter Template',
		});
   },
}
</script>

<style>
@import "../style/reset.css";
@import "../style/font.css";
@import "../style/variables.css";
@import "../style/style.css";
</style>
