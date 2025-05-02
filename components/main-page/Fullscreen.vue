<template>
  <div :class="$style.container">
    <div :class="$style.main">
      <div :class="$style.left">
        <div :class="$style.title">{{ $t("mainPage.fullscreen.title") }}</div>
        <div :class="$style.text">
          {{ $t("mainPage.fullscreen.text") }}
          <span>{{ $t("mainPage.fullscreen.subtext") }}</span>
        </div>
        <div :class="$style.button">{{ $t("mainPage.fullscreen.button") }}</div>
      </div>
      <div :class="$style.right">
        <img src="/images/main-page/ai.png" alt="" />
      </div>
    </div>
  </div>
</template>

<style lang="scss" module>
.container {
  height: calc(100vh - 6rem);
  max-width: 100vw;
  background-color: $bg;
  .main {
    display: grid;
    grid-template-columns: 1fr 1fr;
    @include custom(900) {
      grid-template-columns: 1fr;
    }
    .left {
      padding: 7.5rem 3rem 0 3rem;
      .title {
        font-weight: 700;
        font-size: 4rem;
        color: $white;
        margin: 0 0 1.5rem 0;
        max-width: 37rem;
        @include custom(1200) {
          font-size: 2rem;
          max-width: none;
        }
      }
      .text {
        font-size: 1.25rem;
        line-height: 140%;
        color: $light-blue;
        max-width: 37rem;
        margin: 0 0 3rem 0;
        @include custom(1200) {
          font-size: 1rem;
        }
        span {
          display: block;
          margin-top: 1rem;
        }
      }
      .button {
        padding: 0.75rem 1.5rem;
        display: inline-block;
        border-radius: 0.25rem;
        cursor: pointer;
        color: $white;

        background: linear-gradient(180deg, $main-blue 0%, $purple 100%);
        border: 1px solid;
        border-image-source: linear-gradient(
          135deg,
          $purple 0%,
          $main-blue 100%
        );
        box-shadow: 2px 4px 24px 0px #7d6ceb;
      }
    }
    .right {
      max-width: 100%;
      max-height: 100%;
      @include custom(1200) {
        max-width: 30rem;
        max-height: 30rem;
      }
      @include custom(900) {
        display: none;
      }
      img {
        width: 100%;
        height: 100%;
      }
    }
  }
}
</style>
