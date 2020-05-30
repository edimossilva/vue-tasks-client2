<template>
  <div>
    <h1>Login</h1>
    <div>
      <label>Username:</label>
      <input type="text" @input="username = $event.target.value" />
    </div>
    <div>
      <label>Password:</label>
      <input type="password" autocomplete="new-password" @input="password = $event.target.value" />
    </div>
    <button>Login</button>
    {{username}}
    {{password}}
  </div>
</template>

<script>
export default {
  data() {
    return {
      username: "",
      password: ""
    };
  }
};
</script>


