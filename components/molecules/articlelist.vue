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
  @media screen and (min-width: 768px) {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    padding-bottom: 1.6em;
  }
  &__item{
    font-size: 1.6rem;
    @media screen and (min-width: 768px) {
      width: 32%;
    }
    a{
      display: block;
      position: relative;
      margin-bottom: 1em;
      padding: 0 2em 0 1em;
      border-bottom: 1px #efefef solid;
      text-decoration: none;
      @media screen and (min-width: 768px) {
        margin-bottom: 0;
        padding: 1em 2em 1em 1em;
        border: 1px #efefef solid;
        transition: background .6s ease, color .6s ease;
        &:hover{
          background-color: #000;
          color: #efefef;
        }
      }
      &::before, &::after{
        content: '';
        position: absolute;
        right: 1em;
        top: 50%;
        width: .5em;
        height: .5em;
        margin-top: -.25em;
        border-right: 1px #333 solid;
      }
      &::before{
        transform: rotate(45deg);
      }
      &::after{
        transform: rotate(-45deg);
      }
      dl{
        padding-bottom: 1em;
        @media screen and (min-width: 768px) {
          padding-bottom: 0;
        }
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