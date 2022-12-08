<template>
  <a class="happy-hours-banner" href="#" target="_blank">
    <div class="happy-hours-banner__inner">
      <div class="happy-hours-banner__content">
        <baisad-logo class="happy-hours-banner__logo" />
        <happy-hours-banner-title class="happy-hours-banner__title" />
        <happy-hours-banner-caption class="happy-hours-banner__caption" />
        <happy-hours-banner-button class="happy-hours-banner__button" />
        <happy-hours-banner-rect class="happy-hours-banner__rect_small" />
        <happy-hours-banner-rect class="happy-hours-banner__rect_medium" />
        <happy-hours-banner-rect class="happy-hours-banner__rect_large" />
        <happy-hours-banner-image-gift class="happy-hours-banner__image-gift_small" />
        <happy-hours-banner-image-gift class="happy-hours-banner__image-gift_big" />
        <happy-hours-banner-rating class="happy-hours-banner__rating" />
        <happy-hours-banner-disclaimer class="happy-hours-banner__disclaimer" />
      </div>
    </div>
  </a>
</template>

<script>
import BaisadLogo from './BaisadLogo.vue';
import HappyHoursBannerTitle from './HappyHoursBannerTitle.vue';
import HappyHoursBannerCaption from './HappyHoursBannerCaption.vue';
import HappyHoursBannerButton from './HappyHoursBannerButton.vue';
import HappyHoursBannerRect from './HappyHoursBannerRect.vue';
import HappyHoursBannerImageGift from './HappyHoursBannerImageGift.vue';
import HappyHoursBannerRating from './HappyHoursBannerRating.vue';
import HappyHoursBannerDisclaimer from './HappyHoursBannerDisclaimer.vue';

export default {
  name: 'HappyHoursBanner',
  components: {
    BaisadLogo,
    HappyHoursBannerTitle,
    HappyHoursBannerCaption,
    HappyHoursBannerButton,
    HappyHoursBannerRect,
    HappyHoursBannerImageGift,
    HappyHoursBannerRating,
    HappyHoursBannerDisclaimer,
  },
};
</script>

<style lang="scss">
.happy-hours-banner {
  position: relative;

  display: block;

  width: 100%;
  min-width: 980px;
  height: 250px;

  background: #004ba5;

  overflow: hidden;
  text-decoration: none;

  cursor: pointer;

  &__inner {
    position: absolute;
    right: -720px;
    left: -720px;

    width: 1440px;
    height: 250px;

    margin: 0 auto;

    background-image: linear-gradient(270deg, #004ba5, #00b6f0 31%, #004ba5);
  }

  &__content {
    position: relative;

    width: auto;
    height: 100%;

    margin: 0 auto;
  }

  &__logo {
    position: absolute;
    top: 20px;
    left: 325px
  }

  &__title {
    position: absolute;
    top: 65px;
    left: 325px
  }

  &__caption {
    position: absolute;
    top: 118px;
    left: 325px
  }

  &__button {
    position: absolute;
    top: 170px;
    left: 325px
  }

  &__rect {
    &_small {
      top: 8px;
      left: 848px;
    }

    &_medium {
      top: -28px;
      left: 811px;

      width: 317px;
      height: 317px;
      border-radius: 54px;
    }

    &_large {
      top: -65px;
      left: 775px;

      width: 390px;
      height: 390px;
      border-radius: 82px;
    }
  }

  &__image-gift {
    &_small {
      top: 0;
      left: 806px;

      width: 173px;
      height: 178px;

      background-image: url(@/assets/image/image-2.png);
    }

    &_big {
      top: 14px;
      left: 905px;

      width: 202px;
      height: 225px;

      background-image: url(@/assets/image/image-1.png);
    }
  }

  &__rating {
    position: absolute;
    left: 1091px;
    top: 20px;
  }

  &__disclaimer {
    position: absolute;
    top: 89px;
    left: 325px;
  }
}
</style>
