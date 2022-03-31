<template>
  <aside
    @click="btnMenu"
    class="l-header__hamburgar"
  >
    <img src="~/assets/img/common/bars-solid.svg" alt="menu" width="100" height="100">
  </aside>
</template>

<script>
export default {
  methods: {
    btnMenu () {
      this.$emit('btnMenu')
    }
  }
}
</script>