<template>
  <ul class="l-articlelist">
    <li class="l-articlelist__item">
      <nuxt-link to="/">
        <dl>
          <dt>sample</dt>
          <dd>this is a sample.</dd>
        </dl>
      </nuxt-link>
    </li>
    <li class="l-articlelist__item">
      <nuxt-link to="/">
        <dl>
          <dt>sample</dt>
          <dd>this is a sample.</dd>
        </dl>
      </nuxt-link>
    </li>
    <li class="l-articlelist__item">
      <nuxt-link to="/">
        <dl>
          <dt>sample</dt>
          <dd>this is a sample.</dd>
        </dl>
      </nuxt-link>
    </li>
  </ul>
</template>

<style lang="scss" scoped>
.l-articlelist{
  list-style: none;
  padding-bottom: 1em;
  &__item{
    font-size: 1.6rem;
    a{
      display: block;
      margin-bottom: 1em;
      padding: 0 1em 1em;
      border-bottom: 1px #efefef solid;
      text-decoration: none;
      dl{
        dt{
          padding-bottom: .5em;
          font-size: 1.8rem;
          line-height: 1;
        }
        dd{
          font-size: 1.6rem;
        }
      }
    }
  }
}
</style>