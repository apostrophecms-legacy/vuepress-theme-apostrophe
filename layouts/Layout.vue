<template>
  <ParentLayout>
    <template #sidebar-bottom>
      <section v-if="$themeConfig && $themeConfig.latestVersionPromo"
        class="layout__promo"
      >
        <span>🌟</span>
        <a href="https://v3.docs.apostrophecms.org">Learn About Apostrophe 3</a>
      </section>
    </template>
  </ParentLayout>
</template>

<script>
import ParentLayout from '@parent-theme/layouts/Layout.vue'

export default {
  name: 'Layout',
  components: {
    ParentLayout
  }
}
</script>

<style lang="stylus" scoped>
  .layout__promo
    display: inline-block;
    margin-left: 0.75rem;
    padding: 0.35rem 1rem .35rem 0.5rem;
    border-radius: 10px;
    background-color: #e3dbff;
    font-size: 17px;

    a
      display: inline
      font-weight: 600
      color: inherit

    span
      margin-right: 0.5rem
</style>