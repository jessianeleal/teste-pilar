<template>
    <div class="search_component">
        <input class="search_text" type="text">
        <button><img class="search_img" src="../assets/search.png" alt=""/></button>
    </div>
</template>


<script>
export default {
    name: 'SearchImoveis',
}
</script>

<style>
    .search_component {
        border: 1px solid #000;
        width: 44%;
        display: flex;
        justify-content: space-between;
        padding: 8px;
        align-content: center;
        margin-left: 23px;
    }
    .search_text {
        border: none;
         width: 100%
    }
    input:focus-visible {
        outline: none;
    }
    .search_img {
        width: 15px;
        height: 15px;
    }
    button {
        background: transparent;
        border: none;
    }
    button:hover {
        cursor: pointer;
    }
</style>