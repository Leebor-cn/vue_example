<template>
    <div>
        <h3>hello Bar</h3>
    </div>
</template>

<script>
export default {
  name: 'foo',
  data () {
    return {
      info: null,
      loading: true,
      errored: false
    }
  },
  mounted () {
    this.axios.get('http://127.0.0.1:9902/api/')
      .then(function (response) {
        console.log(response)
      })
  }
}
</script>
