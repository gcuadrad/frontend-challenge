<template>
  <div>
    <error-message :errors="errors" />
    Create User:
    <table>
      <tr>
        <th>Name:</th>
        <th><input v-model="name"></th>
      </tr>
      <tr>
        <th>Lastname:</th>
        <th><input v-model="last_name"></th>
      </tr>
      <tr>
        <th>Email:</th>
        <th><input v-model="email"></th>
      </tr>
      <button v-on:click="createUser">Create User</button>
    </table>
  </div>
</template>

<script>
export default {
  name: 'new-user',
  data () {
    return {
      errors: [],
      name: null,
      last_name: null,
      email: null
    }
  },
  methods: {
    createUser () {
      alert('Under construction!')
      // Axios request example:
      // auth.sendRequest().HTTP_VERB_HERE(URL_HERE, PARAMS_HERE)
      // Required HTML
      // curl --request POST \
      // --url https://reqres.in/api/users \
      // --header 'content-type: application/json' \
      // --data '{
      // "email": "juan@perez.com", "first_name": "Juan", "last_name": "Perez"
      // }'
    }
  }
}
</script>

<style lang="css" scoped>
</style>
