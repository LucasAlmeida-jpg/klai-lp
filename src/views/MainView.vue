<template>
  <div class="container">
   <FirstSection/>
   <SecondSection class="margin-between"/>
   <ThirdSection class="margin-between"/>
   <FourthSection class="margin-between"/>
   <SixthSection class="margin-between"/>
   <SeventhSection class="margin-between"/>
   <EighthSection class="margin-between"/>
   <NinthSection class="margin-between"/>

  </div>
</template>

<script>
import FirstSection from '@/components/FirstSection.vue'
import SecondSection from '@/components/SecondSection.vue'
import ThirdSection from '@/components/ThirdSection.vue'
import FourthSection from '@/components/FourthSection.vue'
import SixthSection from '@/components/SixthSection.vue'
import SeventhSection from '@/components/SeventhSection.vue'
import EighthSection from '@/components/EighthSection.vue'
import NinthSection from '@/components/NinthSection.vue'


export default {
  name: 'App',
  components: {
    FirstSection,
    SecondSection,
    ThirdSection,
    FourthSection,
    SixthSection,
    SeventhSection,
    EighthSection,
    NinthSection
  }
}
</script>


