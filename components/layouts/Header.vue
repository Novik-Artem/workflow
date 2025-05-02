<template>
  <header :class="$style.header">
    <div :class="$style.logo">
      <div :class="$style.icon">
        <img src="/icons/logo.svg" alt="" />
      </div>
      <div :class="$style.title">WORKFLOW <span>tech</span></div>
    </div>
    <div :class="$style.lang">
      <div :class="$style.locale">ru</div>
      <div :class="$style.locale">en</div>
    </div>
  </header>
</template>

<style lang="scss" module>
.header {
  background-color: #140e1b;
  height: 6rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 3rem;
  .logo {
    display: flex;
    align-items: center;
    gap: 0.65625rem;
    .title {
      font-weight: 700;
      font-size: 1.125rem;
      color: white;
      span {
        font-weight: 300;
        font-size: 0.875rem;
        color: #d4e2f6;
      }
    }
  }
  .lang {
    display: flex;
    align-items: center;
    gap: 0.75rem;
    color: #969696;
    text-transform: uppercase;
    .locale {
      padding: 0.75rem;
      border-radius: 0.25rem;
      cursor: pointer;
      &.active {
        cursor: default;
        background: #ffffff14;
        color: white;
      }
    }
  }
}
</style>
