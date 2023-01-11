<script>
import Trabajos from "./trabajos.svelte";
import VistaDefecto from "./vistaDefecto.svelte";

let numeroElecciones = 0;

function eleccion() {
    numeroElecciones = 1;
}

function eleccion2() {
    numeroElecciones = 2;
}

function eleccion3() {
    numeroElecciones = 3;
}
</script>

<div class="container center">

    <div class="row">
        <div class="col">
            <a href="#" class="btn button" on:click={eleccion} ><i class="bi bi-file-earmark-text-fill"></i>
                <h5  >Trabajos</h5></a>
        </div>
        <div class="col">
            <a href="#" class="btn button " on:click={eleccion2} ><i class="bi bi-file-earmark-pdf"></i><h5>CV</h5>
                </div>
                <div class="col">
                    <a href="#" class="btn button" on:click={eleccion3} >
                        <i class="bi bi-envelope-at-fill"></i><h5>Contactame</h5></a>
                </div>

                </div>
                <div class="row">
                    <div class="col">
                    {#if numeroElecciones==1}
                    <Trabajos />
                    <h1>1</h1>
                    {:else if  numeroElecciones==2}
                    <h2>2</h2>
                    {:else if numeroElecciones==3 }
                    <h1>3</h1>
                    {:else}
                    <VistaDefecto />
                    {/if}
                </div>
                    </div >

                </div>

<style>
.bi {
    color: rgb(234, 240, 245);
    font-size: 80px;
}

h5 {
    color: white;
}

.center {
    text-align: center;
}

a:hover {
    background: radial-gradient(circle, rgb(150, 147, 147) 0%, 100%);
    border-radius: 10%;
    box-shadow:
        inset 0 -3em 3em rgba(0, 0, 0, 0.1),
        0 0 0 2px rgb(255, 255, 255),
        0.3em 0.3em 1em rgba(0, 0, 0, 0.3);
    color: rgb(49, 217, 239);
}

i:hover {
    color: rgb(49, 217, 239);
}

h5:hover {
    color: rgb(49, 217, 239);
}
</style>
