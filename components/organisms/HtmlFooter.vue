<template>
  <footer class="l-footer">
    <dl>
      <dt>
        <atomsLogo/>
      </dt>
      <dd>
        <moleculesNavigation/>
      </dd>
    </dl>
    <atomsCopyright/>
  </footer>
</template>

<style lang="scss" scoped>
.l-footer{
  padding: 2.4rem 0;
  background-color: #333;
  dl{
    padding-bottom: 2.4rem;
    dt{
      padding-bottom: 1em;
      color: #efefef;
      font-size: 2rem;
      font-weight: 400;
      line-height: 1;
      text-align: center;
    }
  }
  .l-navigation{
    position: static;
  }
  .c-copyright{
    color: #efefef;
    font-size: 1.2rem;
    text-align: center;
  }
}
</style>