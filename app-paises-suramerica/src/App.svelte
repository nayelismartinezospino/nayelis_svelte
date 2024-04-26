<script>
    import Paises from "./lib/paises.svelte";
    const lista = [
        "Colombia",
        "Venezuela",
        "Ecuador",
        "Peru",
        "Brasil",
        "Paraguay",
        "Bolivia",
        "Uruguay",
        "Argentina",
        "Chile",
    ];
</script>

<div class="main">
    {#each lista as pais}
        <div>
            <Paises {pais} />
        </div>
    {:else}
        No existen elementos
    {/each}
</div>
<svelte:head>
    <title>Paises suramericanos</title>
</svelte:head>

<style>
    .main {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        grid-gap: 10px;
        grid-auto-rows: minmax(100px, auto);
    }
</style>
