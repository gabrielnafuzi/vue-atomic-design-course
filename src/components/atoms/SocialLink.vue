<template>
  <a class="social-link" :href="to" target="_blank" rel="noreferrer noopener">
    <img :src="iconPath" :alt="name" />
  </a>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'SocialLink',
  props: {
    name: { type: String, required: true },
    icon: { type: String, required: true },
    to: { type: String, required: true }
  },
  computed: {
    iconPath(): string {
      return require(`@/assets/images/icons/${this.icon}`)
    }
  }
})
</script>

<style lang="scss" scoped>
.social-link {
  background-color: #ff895f;
  width: 47px;
  height: 47px;
  border-radius: 5rem;
  display: grid;
  justify-items: center;
  align-items: center;
  transition: transform 0.2s linear;

  &:hover {
    transform: scale(1.1);
  }

  img {
    width: 23px;
    height: 23px;
  }
}
</style>
