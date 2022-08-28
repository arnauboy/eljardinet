<script>

    let promise = getTarifes();

    async function getTarifes() {
        const response = await fetch("http://localhost:3000/tarifes"); //Wait for promise
        if (response.ok) {
            const parsedResponse = await response.json(); //Wait for promise
            return parsedResponse;
        }
        else {
            throw new Error("Error al carregar les tarifes");
        }
    }

</script>

<div class="section" >
    <h1> Tarifes </h1>
    {#await promise}
        <p class = "load_message">Carregant tarifes...</p>
    {:then value}
        <div style = "display: flex; margin: 0 auto;">
        {#each value as tarifa}
            <div class = "tarifa">
                <p style = "font-size: 20px; font-weight: bold">{tarifa.name}</p>
                <p> <span style = "font-size: 20px; font-weight: bold">{tarifa.costPerNight} </span> €/nit</p>
                <p> Mínim: {tarifa.n_nights} nits</p>
            </div>
        {/each}
        </div>
    {:catch error}
        <p>{error.message}</p>
    {/await}

</div>
<style>
    .load_message {
        text-align: center;
        font-size: 20px;
    }

    .tarifa{
        border-radius: 10px;
        border-style: solid;
        border-color: green;
        text-align: center;
        max-width: 20%;
        margin: 10px;
        padding: 10px;
    }

    p {

    }
    @media screen and (max-width: 600px) {
        
    }
    
</style>