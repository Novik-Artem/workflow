<template>
  <div :class="$style.container">
    <div :class="$style.main">
      <div :class="$style.left">
        <div :class="$style.title">Готовое решение для вашего бизнесса</div>
        <div :class="$style.text">
          Workflow — это умный инструмент для автоматического соединения
          сервисов, который избавит вас от рутины.
          <span>Автоматизируйте рутину — сосредоточьтесь на главном</span>
        </div>
        <div :class="$style.button">Подключить</div>
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
  background-color: #140e1b;
  .main {
    display: grid;
    grid-template-columns: 1fr 1fr;
    @media (max-width: 900px) {
      grid-template-columns: 1fr;
    }
    .left {
      padding: 7.5rem 3rem 0 3rem;
      .title {
        font-weight: 700;
        font-size: 4rem;
        color: white;
        margin: 0 0 1.5rem 0;
        max-width: 37rem;
        @media (max-width: 1200px) {
          font-size: 2rem;
          max-width: none;
        }
      }
      .text {
        font-weight: 600;
        font-size: 1.25rem;
        line-height: 140%;
        color: #d4e2f6;
        max-width: 37rem;
        margin: 0 0 3rem 0;
        @media (max-width: 1200px) {
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
        color: white;
        font-weight: 600;
        background: linear-gradient(180deg, #523ce1 0%, #7f6eed 100%);
        border: 1px solid;
        border-image-source: linear-gradient(135deg, #7f6eed 0%, #523ce1 100%);
        box-shadow: 2px 4px 24px 0px #7d6ceb;
      }
    }
    .right {
      max-width: 100%;
      max-height: 100%;
      @media (max-width: 1200px) {
        max-width: 30rem;
        max-height: 30rem;
      }
      @media (max-width: 900px) {
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
