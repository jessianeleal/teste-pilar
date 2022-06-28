<template>
    <section class="produtos_imoveis">
        <div v-for="produto in produtos" :key="produto.id" class="lista_imoveis">
            <img :src="produto.image" alt="" class="imagens_imoveis">
            <p class="texto_destaque">{{ produto.address}}, {{ produto.number }}</p>
            <p>{{ produto.city }}</p>
            <p class="texto_destaque">R$ {{ produto.asking_price }}</p>
            <p>{{ produto.bedrooms }}QT {{ produto.suites }}ST {{ produto.parking_spots }}VG</p>
        </div>
    </section>
</template>


<script>
import produtosData from "../api/imoveis.json";

export default {
    name: 'ProdutosImoveis',
    data () {
        return {
            produtos: produtosData
        }
    },
};
</script>

<style>
    .produtos_imoveis {
        display: flex;
        flex-wrap: wrap;
        margin: 15px 5px;
    }
    .lista_imoveis {
        width: 21%;
        border: 1px solid #000;
        margin: 15px 20px;
        text-align: center;
    }
    .imagens_imoveis {
        width: 100%;
        height: 130px;
    }
    .texto_destaque {
        font-weight: bold;
    }
</style>