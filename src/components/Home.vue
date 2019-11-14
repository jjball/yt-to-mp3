<template>
<b-container>
  <b-row align-h="center">
    <b-form @submit="onSubmit" inline>
      <b-form-group
        id="input-group-ytlink"
      >
        <b-row align-h="center">
          <b-col cols="7">
            <b-form-input
              id="input-ytlink"
              class="mb-2 mr-sm-2 mb-sm-0"
              v-model="form.name"
              required
              placeholder="http://www.youtube.com/"
            ></b-form-input>
          </b-col>
          <b-col cols="2">
            <b-button type="submit" variant="primary">Convert</b-button>
          </b-col>
        </b-row>
      </b-form-group>
    </b-form>
  </b-row>
</b-container>
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
