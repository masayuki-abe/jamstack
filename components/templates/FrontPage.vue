<template>
  <main>
    <section class="p-heroimage">
      <h2>Hello...!</h2>
    </section>

    <section class="p-about">
      <div class="f-mixin__inner">
        <h3 class="c-title__section">About</h3>
        <p class="c-text__read p-about__text">I..., I..., I am......</p>
        <p class="c-button__more">
          <nuxt-link to="/about">
            More
          </nuxt-link>
        </p>
      </div>
    </section>

    <section class="p-articlelist">
      <div class="f-mixin__inner">
        <h3 class="c-title__section">News</h3>
        <MoleculesArticlelist />
        <p class="c-button__more">
          <nuxt-link to="/about">
            More
          </nuxt-link>
        </p>
      </div>
    </section>
  </main>
</template>

<style lang="scss" scoped>
.f-mixin{
  &__inner{
    padding: 0 20px 45px;
  }
}
.c-title{
  &__section{
    padding-bottom: .5em;
    font-size: 2.4rem;
    font-weight: 400;
    text-align: center;
  }
}
.c-text{
  &__read{
    font-size: 1.6rem;
  }
}
.c-button{
  &__more{
    width: 30%;
    margin: 0 auto;
    a{
      display: block;
      padding: .5em 1em;
      border: 1px #efefef solid;
      color: #333;
      font-size: 1.6rem;
      line-height: 1;
      text-align: center;
      text-decoration: none;
    }
  }
}
.p-heroimage{
  width: 100%;
  margin-bottom: 45px;
  border-bottom: 1px #efefef solid;
  h2{
    padding: 4em 0;
    color: #fff;
    font-size: 2.4rem;
    line-height: 1;
    letter-spacing: .2em;
    text-align: center;
    text-shadow: 1px 1px #ccc;
  }
}
.p-about{
  &__text{
    padding-bottom: 1em;
    text-align: center;
  }
}
</style>