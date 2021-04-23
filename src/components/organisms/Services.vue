<template>
  <div class="services">
    <Service
      title="Front End"
      description="Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsum eligendi reprehenderit magnam consectetur ipsam unde cupiditate consequatur odio. Nostrum expedita facilis eos similique inventore. Consequuntur temporibus itaque laudantium velit ipsum."
    />
    <Service
      title="Back End"
      description="Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsum eligendi reprehenderit magnam consectetur ipsam unde cupiditate consequatur odio. Nostrum expedita facilis eos similique inventore. Consequuntur temporibus itaque laudantium velit ipsum."
    />
    <Service
      title="Manutenção"
      description="Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsum eligendi reprehenderit magnam consectetur ipsam unde cupiditate consequatur odio. Nostrum expedita facilis eos similique inventore. Consequuntur temporibus itaque laudantium velit ipsum."
    />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { Service } from '@/components/molecules'

export default defineComponent({
  name: 'Services',
  components: {
    Service
  }
})
</script>

<style lang="scss" scoped>
.services {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 5rem;
}
</style>
