<template>
<div>
<main class="container">
    <AppHeader />
    <AppRestaurantInfo :dataSource="fooddata"/>
  </main>
  <AppFooter />
</div>
  
</template>

<script>
import AppHeader from '@/components/AppHeader.vue';
import AppRestaurantInfo from '@/components/AppRestaurantInfo.vue';
import AppFooter from '@/components/AppFooter.vue';
import { mapState } from 'vuex';

export default {
  components: {
    AppHeader,
    AppRestaurantInfo,
    AppFooter
  },
    computed: {
    ...mapState([
      'fooddata',
    ])
  }
}
</script>
