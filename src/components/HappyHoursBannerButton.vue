<template>
  <div class="lock-button">
    <icon-lock />
    <lock-button-text />
  </div>
</template>

<script>
import IconLock from './IconLock.vue';
import LockButtonText from './LockButtonText.vue';

export default {
  name: 'BannerButton',
  components: {
    IconLock,
    LockButtonText,
  },
};
</script>

<style lang="scss">
.lock-button {
  display: flex;
  justify-content: center;
  align-items: center;

  width: 256px;
  height: 56px;

  background-color: #e61c2d;
  border-radius: 100px;
  box-shadow: 0 3px 0 #b31623;

  opacity: 0;

  &__text {
    margin: 0 0 0 9px;
  }
}
</style>
