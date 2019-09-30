<script>
    import InfoIcon from "../iconos/InfoIcon.svelte";
    import TituloAyuda from "../iconos/TituloAyuda.svelte";
</script>

<style>

        /* * {
            outline: 1px solid blue;
        } */

        article {
            max-width: 360px;
            max-height: 420px;
            background-color: rgb(255, 255, 255);
        }

        .Informacion {
            max-width: 32%;
            display: flex;
            align-items: center;
            flex-direction: column;
        }

        .Encabezado {
            width: 100%;
            height: 9rem;
            background: #516980;
            box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.1);
            border-radius: 0px 0px 0px 40px;
        }

        .Acerca {
            padding: 2rem;
        }

        .Texto {
            width: 100%;
            max-height: 20rem;
            overflow-y: auto;
            color: #5E5E5E;
            font-style: normal;
            font-weight: normal;
            font-size: 1rem;
            line-height: 1.5rem;
        }

        .Subtitulo {
            font-style: normal;
            font-weight: normal;
            font-size: 1.5rem;
            color: #878787;
        }

        .Mapa {
            padding-top: 1.5rem;
        }

        .Informa {
            margin-top: -5.6rem;
            margin-left: 30rem;
        }
        
    
</style>
    
<article class="Informacion">
    <header class="Encabezado">
        <figure class="Mapa">
            <TituloAyuda/>
        </figure>
        <figure class="Informa">
            <InfoIcon/>
        </figure>
    </header>
    <div class="Acerca">
        <p class="Subtitulo">
            ACERCA DE 
        </p>
        <div class="Texto">
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Sapiente quod quidem delectus hic aspernatur sit eum rem laborum sequi, recusandae similique ut totam, dolores dignissimos veniam. Voluptatem error ipsam ipsa!
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Assumenda veritatis hic illo dolore a voluptate perspiciatis, beatae nisi odit distinctio maiores reiciendis corporis obcaecati veniam, illum possimus at? Delectus, vitae.
            </p>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Impedit maxime quisquam optio quis aut nihil vero, ex fugiat non totam quidem modi, suscipit laboriosam molestiae placeat eligendi vel qui perspiciatis!
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Impedit maxime quisquam optio quis aut nihil vero, ex fugiat non totam quidem modi, suscipit laboriosam molestiae placeat eligendi vel qui perspiciatis!
            </p>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quo consequuntur autem repudiandae ducimus nobis possimus facere sunt sint vero laudantium ex aperiam ipsa a, beatae neque, nostrum dolor animi sit!
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quo consequuntur autem repudiandae ducimus nobis possimus facere sunt sint vero laudantium ex aperiam ipsa a, beatae neque, nostrum dolor animi sit!
            </p>
        </div>
    </div>
</article>