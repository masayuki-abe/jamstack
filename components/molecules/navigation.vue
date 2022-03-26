<template>
  <nav class="l-navigation">
    <ul clas="l-navigation__body">
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
  &__body{
    list-style: none;
    &-item{
      font-size: 1.6rem;
      line-height: 1;
      a{
        display: block;
        padding: 1em;
        color: #efefef;
        text-decoration: none;
        text-align: center;
      }
    }
  }
}
</style>