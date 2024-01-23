<template>
  <div class="home">
    <Header />
    <Milliard />
    <Description />
    <CTab />
  </div>
</template>

<script>
import Header from '@/components/Header'
import Milliard from '@/components/Milliard'
import Description from '@/components/Description'
import CTab from '@/components/CTab'

export default {
  name: 'HomeView',
  components: {
    Header,
    Milliard,
    Description,
    CTab
  }
}
</script>
