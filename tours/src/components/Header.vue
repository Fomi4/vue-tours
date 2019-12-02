<template lang="html">
  <header>
    <img src="./../assets/logo.png" width="50" alt="">
    <p>Welcome to the application</p>
    <nav>
      <ul class="nav">
        <li><a href="#">Home</a></li>
        <li><a href="#">Services</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Contact Us</a></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style lang="css" scoped>
.nav {
  display: flex;
  justify-content: space-around;
  padding: 0;
  margin: 0;
  list-style: none;
}

.nav a {
  color: cadetblue;
}
</style>