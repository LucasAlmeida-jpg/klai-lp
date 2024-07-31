<template>
  <div class="container">
   <Banner />
   <AbstractInfo class="margin-scoped" />
  </div>
</template>

<script>
import Banner from '@/components/Banner.vue'
import AbstractInfo from '@/components/Abstract.vue'


export default {
  name: 'App',
  components: {
    Banner,
    AbstractInfo
  }
}
</script>


