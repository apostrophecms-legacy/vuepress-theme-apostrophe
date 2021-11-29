<template>
  <ParentLayout>
    <template #sidebar-bottom>
      <section v-if="$themeConfig && $themeConfig.latestVersionPromo"
        class="layout-note"
      >
        <p>
          <a href="https://v3.docs.apostrophecms.org/">Learn about Apostrophe 3. 🆕</a>
        </p>
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
  .layout-note
    background-color: $badgeTipColor
    padding 0.35rem 1rem 0.35rem 1.25rem

    a
      color: white
</style>