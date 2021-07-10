<template>
  <form>
    <div class="busca-container">
      <input type="text" id="busca" name="busca" v-model="busca" placeholder="Buscar..." />
      <input type="submit" id="lupa" value="Buscar" @click.prevent="buscarProdutos" />
    </div>
  </form>
</template>

<script>
export default {
  data() {
    return {
      busca: "",
    };
  },
  methods: {
    buscarProdutos() {
      this.$router.push({ query: { q: this.busca } });
    },
  },
};
</script>

<style scoped>
form {
  max-width: 600px;
  margin: 30px auto 60px auto;
  position: relative;
}

#busca {
  width: 100%;

  padding: 20px;
  border: none;
}
.busca-container {
  transition: all 0.4s;
}
.busca-container:hover,
.busca-container:focus {
  transform: scale(1.1);
}

#lupa {
  width: 62px;
  height: 62px;
  background: url("../assets/search.svg") no-repeat center center;
  text-indent: -300px;
  cursor: pointer;
  border: none;
  position: absolute;
  top: 0px;
  right: 0px;
  box-shadow: none;
}
</style>
