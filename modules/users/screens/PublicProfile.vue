<script setup lang="ts">
import PublicHeadline from '../components/PublicHeadline/PublicHeadline.vue'
import WidgetGroup from '../components/Widget/Group/Group.vue'
import WidgetGroupLoader from '../components/Widget/Group/Loader.vue'
import WidgetCondensed from '../components/Widget/Condensed/Condensed.vue'
</script>

<template>
  <PublicHeadline />

  <WidgetGroup>
    <WidgetGroupLoader :loading="true" :amount="3">
      <WidgetCondensed :value="10" label="Gists no total" />
      <WidgetCondensed :value="5" label="Gists gratuitos" />
      <WidgetCondensed :value="5" label="Gists pagos" />
    </WidgetGroupLoader>
  </WidgetGroup>
</template>
