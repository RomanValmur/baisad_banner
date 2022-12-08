<template>
  <div class="happy-hours-banner-rect">
  </div>
</template>

<script>
export default {
  name: 'HappyHoursBannerRect',
};
</script>

<style lang="scss">
.happy-hours-banner-rect {
  width: 243px;
  height: 243px;

  border-radius: 38.2px;

  position: absolute;
  background-color: hsla(0, 0%, 100%, 0.1);
  transform: rotate(45deg) scaleX(1);

  opacity: 0;
}
</style>
