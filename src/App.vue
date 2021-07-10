<template>
  <div id="app">
    <AppHeader />
    <main>
      <router-view />
    </main>
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from "@/components/AppHeader.vue";
import AppFooter from "@/components/AppFooter.vue";

export default {
  components: {
    AppHeader,
    AppFooter,
  },
};
</script>
<style>
* {
  box-sizing: border-box;
}

#app {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}
main {
  flex: 1;
}
body,
ul,
li,
h1,
h2,
p {
  padding: 0px;
  margin: 0px;
}
ul {
  list-style: none;
}

body {
  font-family: Helvetica, Arial, sans-serif;
  color: #345;
  background: url("./assets/pattern.svg") repeat top;
}

a {
  color: #345;
  text-decoration: none;
}
img {
  max-width: 100%;
  display: block;
}

.btn {
  display: block;
  background: rgb(86, 179, 40);
  color: white;
  padding: 10px 30px;
  font-size: 1rem;
  font-family: Helvetica, Arial, sans-serif;
  text-align: center;
  border-radius: 4px;
  box-shadow: 0 4px 8px rgba(18, 190, 41, 0.2);
  transition: all 0.3s;
  border: none;
  cursor: pointer;
}

.btn:hover {
  background: rgb(64, 133, 30);
  transform: scale(1.1);
}

input,
textarea {
  border-radius: 4px;
  border: 1px solid white;
  padding: 15px;
  box-shadow: 0 4px 8px rgba(30, 60, 90, 0.1);
  font-size: 1rem;
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  margin-bottom: 15px;
}
input:hover,
input:focus,
textarea:hover,
textarea:focus {
  outline: none;
  box-shadow: 0 6px 12px rgba(30, 60, 90, 0.2);
  border-color: rgba(18, 190, 41, 0.2);
}
</style>
