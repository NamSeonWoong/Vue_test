<template>
    <v-btn @click="test">테스트</v-btn>
</template>

<script>

import axios from "axios"

export default {
    methods:    {
        test()  {
            
// Make a request for a user with a given ID
axios
    .get('https://reqres.in/api')
  .then(res => {
    // handle success
    console.log(res);
  })
  .catch(err => {
    // handle error
    console.log(err);
  })
  .then(()  => {
    // always executed
    console.log("test")
  });
        }
    }
}
</script>

<style>

</style>