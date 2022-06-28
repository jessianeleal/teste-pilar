<template>
    <div class="ordem_component">
       <select name="ordemImoveis" id="ordem" class="ordem_opcoes">
            <option value="valor1" selected>Mais caros</option>
            <option value="valor2">Mais baratos</option>
       </select>
    </div>
</template>


<script>
export default {
    name: 'OrdemImoveis',
}
</script>

<style>
    .ordem_component {
        border: 1px solid #000;
        width: 19.5%;
        display: flex;
        justify-content: space-between;
        padding: 8px;
        align-content: center;
        border-radius: 5px;
    }
    select {
        display: flex;
        justify-content: space-between;
        width: 100%;
    }
    .ordem_opcoes {
        border: none;
    }
</style>