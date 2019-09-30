<script>

</script>

<style>
    .Agrupacion {
        width: 100%;
        height: 4rem;
        margin: 1rem;
        padding: 0 1rem;
        background: #FFFFFF;
        border: 1px solid #DBDBDB;
        box-sizing: border-box;
        box-shadow: 4px 4px 6px rgba(0, 0, 0, 0.06);
        border-radius: 4px;
        display: flex;
        flex-direction: row;
        flex-wrap: nowrap;
        justify-content: space-between;
    }

    .Agrupacion > * {
        padding: 0 1rem;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .Nombre {
        flex-grow: 1;   
        font-size: 1rem; 
        justify-content: flex-start !important;
    }

    .Riesgo {
        display: flex;
        align-items: center;
        justify-content: center;
        flex-shrink: 1;
    }

    .Hablantes {
        flex-shrink: 1;
        display: flex;
        flex-direction: column;
        align-items: space-evenly;
        justify-content: center;
        color: #454344;
    }

    #IconRiesgo {
        color: #e6aa30f2;
    }

</style>

<article class="Agrupacion">
    <div class="Nombre">
        <span>
            Nayeeri (Cora)
        </span>
    </div>
    <div class="Riesgo">
        <i id="IconRiesgo" class="fas fa-exclamation-circle fa-lg"></i>
    </div>
    <div class="Hablantes">
        <span class="Numero">
            28, 718
        </span>
        <span class="Leyenda">
            hablantes
        </span>
    </div>
</article>