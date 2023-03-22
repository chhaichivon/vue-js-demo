<body>
 <h2>About</h2>
</body>
<template>
     <div v-html="htmlString"></div>

  </template>
  
  <script>
    export default {
        name: 'AboutMe',
    }
  </script>

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
