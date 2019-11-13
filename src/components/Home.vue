<template>
  <b-form @submit="onSubmit" inline>
    <b-form-input
      id="input-ytlink"
      class="mb-2 mr-sm-2 mb-sm-0"
      v-model="form.name"
      required
      placeholder="http://www.youtube.com/"
    ></b-form-input>

    <b-button type="submit" variant="primary">Convert</b-button>
  </b-form>
</template>

<script>
// import axios from 'axios';

export default {
  name: 'Home',
  data() {
    return {
      form: {
        ytlink: '',
      },
    }
  },
  methods: {
    onSubmit(evt) {
    evt.preventDefault();
      alert(JSON.stringify(this.form));
      // const resp = axios.post(`/convert?url=${JSON.stringify(form.ytlink)}`);
    },
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
