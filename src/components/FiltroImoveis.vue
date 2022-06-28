<template>
    <div class="filtro_component">
       <select name="filtroImoveis" id="filtro" class="filtro_opcoes">
            <option class="teste" value="valor1" selected>Ativos</option>
            <option value="valor2">Inativos</option>
            <option value="valor2">Todos</option>
       </select>
    </div>
</template>


<script>

export default {
    name: 'FiltroImoveis'
}
</script>

<style>
    .filtro_component {
        border: 1px solid #000;
        width: 19.5%;
        display: flex;
        justify-content: space-between;
        padding: 8px;
        align-content: center;
        border-radius: 5px;
        margin-right: 23px;
    }
    .filtro_opcoes {
        border: none;
    }
    select:focus-visible {
        outline: none;
    }
    .teste {
        padding: 30px;
    }
</style>