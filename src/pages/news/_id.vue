<template>
  <div>IDは{{ $route.params.id }}です</div>
</template>

<script lang="ts">
import { Vue, Component } from 'nuxt-property-decorator'

@Component({})
export default class extends Vue { }
</script>