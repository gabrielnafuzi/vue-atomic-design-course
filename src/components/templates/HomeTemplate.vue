<template>
  <Container class="home-template">
    <Header />
    <Presentation />
    <Services />
  </Container>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { Container } from '@/components/bosons'
import { Header, Presentation, Services } from '@/components/organisms'

export default defineComponent({
  name: 'HomeTemplate',
  components: {
    Container,
    Header,
    Presentation,
    Services
  }
})
</script>

<style lang="scss" scoped>
.home-template {
  margin: 5rem auto;
  display: grid;
  gap: 5rem;
}
</style>
