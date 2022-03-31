<template>
  <main>
    <section class="p-heroimage">
      <h2>News</h2>
    </section>

    <section class="p-articlelist">
      <div class="f-mixin__inner">
        <h3 class="c-title__section">News</h3>
        <MoleculesArticlelist />
      </div>
    </section>
  </main>
</template>

<style lang="scss" scoped>
.f-mixin{
  &__inner{
    padding: 0 20px 45px;
    @media screen and (min-width: 768px) {
      width: 90%;
      max-width: 960px;
      margin: 0 auto;
      padding: 0 0 64px;
    }
  }
}
.c-title{
  &__section{
    padding-bottom: .5em;
    font-size: 2.4rem;
    font-weight: 400;
    text-align: center;
    @media screen and (min-width: 768px) {
      padding-bottom: 1em;
      letter-spacing: .2em;
    }
  }
  &__term{
    padding-bottom: 1em;
    font-size: 2rem;
    font-weight: 600;
    text-align: center;
  }
}
.c-text{
  &__read{
    font-size: 1.6rem;
  }
}
.p-heroimage{
  width: 100%;
  margin-bottom: 45px;
  border-bottom: 1px #efefef solid;
  @media screen and (min-width: 768px) {
    margin-bottom: 64px;
  }
  h2{
    padding: 1.5em 0;
    color: #fff;
    font-size: 2.4rem;
    line-height: 1;
    letter-spacing: .2em;
    text-align: center;
    text-shadow: 1px 1px #ccc;
    @media screen and (min-width: 768px) {
      font-size: 4rem;
    }
  }
}
.p-about{
  &__box01{
    &--dlist{
      .c-text__read{
        text-align: center;
      }
    }
  }
}
</style>