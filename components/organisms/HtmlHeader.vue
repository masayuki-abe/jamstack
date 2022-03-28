<template>
  <header class="l-header">
    <div class="f-mixin__inner">
      <h1 class="l-header__logo">
        <AtomsLogo/>
      </h1>
      <AtomsButtonsBtnHamburger
        @btnMenu="toggleMenu"
      />
      <transition
        @before-enter="beforeEnter"
        @enter="enter"
        @before-leave="beforeLeave"
        @leave="leave"
      >
        <MoleculesNavigation
          v-if="gnaviOn || !isMobile"
        />
      </transition>
    </div>
  </header>
</template>

<script>
export default {
  data () {
    return {
      gnaviOn: false,
      windowWidth: 1025
    }
  },
  computed: {
    isMobile () {
      return this.windowWidth < 1024
    }
  },
  mounted () {
    this.windowWidth = window.innerWidth
    this.$nextTick(() => {
      window.addEventListener('resize', () => {
        this.windowWidth = window.innerWidth
      })
    })
  },
  methods: {
    toggleMenu () {
      this.gnaviOn = !this.gnaviOn
    },
    beforeEnter (el) {
      el.style.height = '0'
    },
    enter (el) {
      el.style.height = el.scrollHeight + 'px'
    },
    beforeLeave (el) {
      el.style.height = el.scrollHeight + 'px'
    },
    leave (el) {
      el.style.height = '0'
    }
  }
}
</script>

<style lang="scss" scoped>
.f-mixin__inner{
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 20px;
  @media screen and (min-width: 768px) {
    width: 90%;
    max-width: 960px;
    margin: 0 auto;
  }
}
.l-header{
  position: relative;
  background-color: #242d20;
  &__logo{
    color: #000;
    font-size: 2.4rem;
    font-weight: 400;
    line-height: 1;
    letter-spacing: .15em;
  }
  &__hamburgar{
    width: 40px;
    font-size: 0;
    line-height: 0;
    @media screen and (min-width: 768px) {
      display: none;
    }
  }
}
</style>