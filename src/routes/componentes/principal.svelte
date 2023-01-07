<script>
    import Formulario from "./formulario.svelte";
</script>
<div class="container">
    <div class="row ">
        <div class="col-xl-4 col-lg-7 col-md-12 ">
            <figure class="figure py-3 mt-5">
                <img src="https://cdn.pixabay.com/photo/2013/01/05/21/02/art-74050_1280.jpg" class="figure-caption img-fluid rounded" alt="yop">
            </figure>
        </div>
        <div class="col text-center fw-bold" >
            <h1 class="nombre py-3">
                Félix Santiago Martinez Pérez
            </h1>
            <h5 class="nombre">Programador:)</h5>
            <p class="font-1 fst-italic  py-4"> Me interesa el desarrollo de funcionalidades que den soluciones a problemas de la vida diaria y laboral.
            En este momento he realizado trabajos como se muestran en mi portafolio con ello he ganando experiencia y un interés a seguir mejorando cada día más.</p>

                <Formulario/>
        </div>
    </div>
</div>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Bowlby+One+SC&family=Orbitron&display=swap');
.font-1 {
    font-family: 'Orbitron', sans-serif;
    font-weight: 400;
   color: white; 
}
.nombre {
    font-family: 'Bowlby One SC', cursive;
    font-weight: 400;
    color: white;
    animation-duration: 3s;
    animation-name: nombreCompleto;
}

@keyframes nombreCompleto {
    from {
        margin-left: 100%;
        width: 300%
    }

    to {
        margin-left: 0%;
        width: 100%;
    }
}
img{
    box-shadow: -5px 5px 20px rgb(255, 255, 255);
}
</style>
