<template>
  <happy-hours-banner :class="{ animated: isAnimated }"/>
</template>

<script>
import HappyHoursBanner from './components/HappyHoursBanner.vue';

export default {
  name: 'App',
  components: {
    HappyHoursBanner,
  },
  data() {
    return {
      isAnimated: true,
    };
  },
  methods: {
    loopAnimation() {
      setInterval(() => {
        this.isAnimated = false;
        setTimeout(() => {
          this.isAnimated = true;
        }, 50);
      }, 11000);
    },
  },
  mounted() {
    this.loopAnimation();
  },
};
</script>

<style lang="scss">
</style>
