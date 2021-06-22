<template>
  <section>
    <h1>Compre ou venda</h1>
    <ProdutosBuscar />
    <ProdutosLista />
  </section>
</template>

<script>
import ProdutosBuscar from "@/components/ProdutosBuscar";
import ProdutosLista from "@/components/ProdutosLista";

export default {
  name: "Home",
  components: {
    ProdutosBuscar,
    ProdutosLista,
  },
};
</script>

<style scoped>
h1 {
  font-size: 2rem;
  color: #40851e;
  text-align: center;
  margin-top: 3rem;
}
</style>
