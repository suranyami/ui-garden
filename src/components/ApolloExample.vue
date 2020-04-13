<template>
  <div class="apollo-example">
    <ApolloQuery
      :query="require('../graphql/Countries.gql')"
    >
      <div slot-scope="{ result: { data } }">
        <template v-if="data">
          <div
            v-for="country of data.countries"
            :key="country.code"
            class="country"
          >
            {{ country.name }}
          </div>
        </template>
      </div>
    </ApolloQuery>
  </div>
</template>

<script>
export default {
  data () {
    return {
    }
  },

  apollo: {
  },

  computed: {
  },

  methods: {
  },
}
</script>

<style scoped>
.form,
.input,
.apollo,
.message {
  padding: 12px;
}

.error {
  color: red;
}

</style>
