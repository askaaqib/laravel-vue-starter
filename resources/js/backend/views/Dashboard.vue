<template>
  <div>
    <b-row>
      <b-col xl="6">
        Dashboard
      </b-col>
    </b-row>
  </div>
</template>

<script>
import axios from 'axios'

export default {
  name: 'Dashboard',
  data() {
    return {
      post_fields: {
        title: { label: this.$t('validation.attributes.title') },
        status: { label: this.$t('validation.attributes.status') },
        pinned: { label: this.$t('validation.attributes.pinned') },
        summary: { label: this.$t('validation.attributes.summary') },
        published_at: {
          label: this.$t('validation.attributes.published_at'),
          class: 'text-center'
        }
      },
      posts: []
    }
  }
}
</script>
