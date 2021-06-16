<template>
  <header>
    <nav>
      <router-link to="/" class="logo"><img src="@/assets/ranek.svg" alt="logo"/></router-link>
      <router-link class="btn" to="/login">Vender / Login</router-link>
    </nav>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
};
</script>

<style scoped>
nav {
  display: flex;
  flex-direction: row;
  padding: 15px 20px;
  width: 100%;
  align-items: center;
  justify-content: space-between;
  box-shadow: 0 2px 4px rgba(18, 190, 41, 0.2);
}

.logo {
  padding: 10px 0;
}

.logo img {
  width: 5.7rem;
}
</style>
