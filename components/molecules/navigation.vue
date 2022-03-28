<template>
  <nav class="l-navigation">
    <ul class="l-navigation__body">
      <li class="l-navigation__body-item">
        <nuxt-link to="/">
          home
        </nuxt-link>
      </li>
      <li class="l-navigation__body-item">
        <nuxt-link to="/about/">
          about
        </nuxt-link>
      </li>
      <li class="l-navigation__body-item">
        <nuxt-link to="/news/">
          news
        </nuxt-link>
      </li>
    </ul>
  </nav>
</template>

<style lang="scss" scoped>
.l-navigation{
  position: absolute;
  top: 100%;
  left: 0;
  z-index: 2;
  width: 100%;
  background-color: rgba(36, 45, 32, .7);
  @media screen and (min-width: 768px) {
    position: static;
    width: auto;
    background-color: transparent;
  }
  &__body{
    list-style: none;
    @media screen and (min-width: 768px) {
      display: flex;
      align-items: center;
      justify-content: center;
    }
    &-item{
      font-size: 1.6rem;
      line-height: 1;
      @media screen and (min-width: 768px) {
        margin: 1em;
      }
      a{
        display: block;
        padding: 1em;
        color: #efefef;
        text-decoration: none;
        text-align: center;
        @media screen and (min-width: 768px) {
          display: inline;
          padding: 0;
          &:hover{
            text-decoration: underline;
          }
        }
      }
    }
  }
}
</style>