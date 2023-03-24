<template>
    
    <div class="login-container">
    <form @submit.prevent="login" class="login-form">
      <label>Username:</label>
      <input type="text" v-model="username">
      <br>
      <label>Password:</label>
      <input type="password" v-model="password">
      <br>
      <button type="submit">Login</button>
    </form>
  </div>

</template>
<script>

export default {
  name: 'Login-Page',
  data() {
    return {
      username: '',
      password: ''
    }
  },
  methods: {
    login() {
      // Replace this with your actual login code
      if (this.username === 'myusername' && this.password === 'mypassword') {
        alert('Logged in successfully!');

      } else {
        alert('Invalid username or password')
      }
    }
  }
}
</script>

<style scoped>
.login-container {
  position: relative;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

.login-form {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
</style>