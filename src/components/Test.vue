<template>
  <div class="test">
    <h1> {{title}} </h1>
    <p>{{user.first_name}}</p>
    <p v-if="show" v-text="user.address"></p>
    <p v-else>Cannot show information</p>
  </div>
</template>

<script>
  export default {
    name : 'test',
    data () {
      return {
        title: 'Hello?',
        user: {
          first_name: 'James',
          address: 'New York, 25148, St. Park'
        },
        show: true

      }

    }
  }

</script>
