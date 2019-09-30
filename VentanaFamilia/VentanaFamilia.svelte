<script>
    import Agrupacion from "./Agrupacion.svelte";
    import BotonCerrar from "../botones/BotonCerrar.svelte";
    import FamiliaDetalle from "./FamiliaDetalle.svelte";



    let elemento = { activo: false };
	const Mostrar = () => {
		elemento.activo = !elemento.activo;
    }
    
</script>

<style>

    article {
        max-width: 360px;
        max-height: 420px;
	}

    .Familia {
        max-width: 35%;
        background: #F7F7F7;
        border-radius: 10px;
	    display: flex;
	    justify-content: center;
        align-items: center;
        flex-direction: column;
        flex-wrap: nowrap;
        justify-content: space-between;
        max-height: 48rem;
    }

    .Encabezado {
        margin-top: -3rem;
    }

    .Contenedor-1 {
        display: flex;
        align-items: center;
        flex-direction: column;
        /* flex-wrap: nowrap; */
        /* justify-content: space-between; */
        overflow-y: auto;
        
    }

    .Cerrar {
        margin-left: 36rem;
        border: 0;
        background-color: #F7F7F7;
        padding: 1rem;
    }

    i {
        color: #bababa;
    }

    img {
		width: 580px;
		height: 455px;
        object-fit: cover;
        box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
        border-radius: 5px;
    }
    
    .Titulo {
        text-align: center;
        font-weight: 200;
        font-size: 1.5rem;
        line-height: 1rem;
        letter-spacing: 0.5rem;
        color: #454344;
        margin: 0.5rem;
    }

    .Principal {
        text-align: center;
        font-weight: 600;
        font-size: 2.5rem;
        line-height: 3rem;
        text-align: center;
        color: #E6AA30;
        margin: 0.5rem;
    }

    .Saber {
        width: 17%;
        height: 10%;
        border: 1px solid #E6AA30;
        box-sizing: border-box;
        border-radius: 15px;
        color: #E6AA30;
    }

    .TitulosLista {
        display: flex;
        justify-content: space-between;
        margin-right: -6rem;
        margin-left: -6rem;
    }

    .TextoFotos {
        position: relative;
        top: -16%;
        left: -39%;
        color: #fff;
    }

    .Flecha {
        width: 50%;
        margin-left: 10rem;
    }

    .Carrousel {
        margin-top: -4.5rem;
        font-size: 0.5rem;
    }

    .Contenedor-2 {
        width: 100%;
        margin-top: 1rem;
    }

    .FamiliaDetalle {
        position: absolute;
        left: 35.1%;
        top: 0.6%;
    }

    .Lista {
        margin-right: -5rem;
        margin-left: -9.5rem;
    }

    #Point {
        padding: 0 .5rem 0 0;
    }


</style>

<article class="Familia">
    <button class="Cerrar">
        <i class="far fa-times-circle fa-2x"></i>
    </button>
    <header class="Encabezado">
        <p class="Titulo">
            FAMILIA
        </p>
        <h1 class="Principal">
            Yuto-nahua
        </h1>
    </header>
        {#if elemento.activo}
	    <button class="Saber" on:click={Mostrar}>
	    	Saber más
	    </button>
        <div class="FamiliaDetalle">
	        <FamiliaDetalle/>
        </div>
        {/if}

        {#if !elemento.activo}
	    <button class="Saber" on:click={Mostrar}>
	    	Saber más
	    </button>
        {/if}
        <div class="Contenedor-1">
	        <img class="Imagen" src={`http://unsplash.it/300/${100+Math.floor(Math.random()*500)}`} alt="img"/>
            <div class="TextoFotos">
                <p>
                    Titulo Foto
                </p>
                <p>
                    Descripción
                </p>
            </div>

            <div class="Carrousel">
                <i id="Point" class="fas fa-circle fa-xs"></i>
                <i id="Point" class="fas fa-circle fa-xs"></i>
                <i id="Point" class="fas fa-circle fa-xs"></i>
                <i id="Point" class="fas fa-circle fa-xs"></i>
                <i id="Point" class="fas fa-circle fa-xs"></i>
                <i id="Point" class="fas fa-circle fa-xs"></i>
                <i id="Point" class="fas fa-circle fa-xs"></i>
                <i id="Point" class="fas fa-circle fa-xs"></i>
                <i id="Point" class="fas fa-circle fa-xs"></i>
            </div>

            <article class="Contenedor-2">
                <span class="Flecha">
                    <i class="fas fa-chevron-down fa-3x"></i>
                </span>
                <header class="TitulosLista">
                    <h4>
                        Agrupaciones Lingüísticas
                    </h4>
                    <h4>
                        Riesgo de desaparición
                    </h4>
                </header>
                    <section class="Lista">
                        <ul>
                        <Agrupacion/>
                        <Agrupacion/>
                        <Agrupacion/>
                        </ul>
                    </section>
            </article>
        </div>
</article>









