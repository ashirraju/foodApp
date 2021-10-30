<template>
<div>
<main class="container">
    <AppHeader />
    <AppRestaurantInfo />
  </main>
  <AppFooter />
</div>
  
</template>

<script>
import AppHeader from '@/components/AppHeader.vue';
import AppRestaurantInfo from '@/components/AppRestaurantInfo.vue';
import AppFooter from '@/components/AppFooter.vue';
export default {
  components: {
    AppHeader,
    AppRestaurantInfo,
    AppFooter
  }
}
</script>
