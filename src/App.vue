<template>
  <section>
    <div class="header_imoveis">
      <SearchImoveis/>
      <OrdemImoveis/>
      <FiltroImoveis/>
    </div>
    <div>
      <ProdutosImoveis/>
    </div>
  </section>
</template>

<script>

import SearchImoveis from './components/SearchImoveis.vue'
import OrdemImoveis from './components/OrdemImoveis.vue'
import FiltroImoveis from './components/FiltroImoveis.vue'
import ProdutosImoveis from './components/ProdutosImoveis.vue'

export default {
  name: 'App',
  components: {
    SearchImoveis, 
    OrdemImoveis,
    FiltroImoveis,
    ProdutosImoveis
  },
}
</script>

<style>
  body {
    margin: 2% 15% 0 15%;
    font-family: 'Inter', sans-serif;
    font-size: 14px;
  }
  .header_imoveis {
    display: flex ;
    justify-content: space-between;
  }
  
</style>
