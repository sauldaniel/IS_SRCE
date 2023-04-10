<template>
    <div class="container">
        <NavBar/>
        
        <div class="graficas">

            <div class="grafica">
                <graficaPie/>
            </div>
            <div class="info">
                <H1>Rendimiento académico</H1>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Magni, facilis similique obcaecati quae officia illo blanditiis, nulla nemo at fugiat in amet sit? In cumque aperiam itaque maiores neque consectetur! </p>
            </div>
            
        </div>

        <div class="modulos">
            <tarjetaModulo moduleName="Módulo de evaluación de AE." moduleDescription="Realizar evaluaciones sobre los atributos de egreso previamente añadidos." redirect="#"
            rutaIMG="https://upload.wikimedia.org/wikipedia/commons/0/08/Feedback-g95f96811e_1920.jpg"/>
            <tarjetaModulo moduleName="Módulo de gestión de AE." moduleDescription="Gestiona las clases que se vincularon al sistema y los atributos de egreso que deseas evaluar." redirect="#"
            rutaIMG="https://upload.wikimedia.org/wikipedia/commons/0/08/Feedback-g95f96811e_1920.jpg"/>
            <tarjetaModulo moduleName="Módulo de gestión de clases" moduleDescription="Gestiona todas las clases que requieran evaluar AE." redirect="#"
            rutaIMG="https://nivelesdeorganizacion.com/wp-content/uploads/2021/07/materias-2.png"/>
        </div>
    </div>
</template>

<script>
import NavBar from '../components/NavBar.vue'
import graficaPie from '../components/graficaPie.vue'
import tarjetaModulo from '../components/tarjetaModulo.vue'

export default {
  name: 'DashboardPage',
  components: {
    NavBar,
    graficaPie,
    tarjetaModulo
  }
}


</script>

<style>
.container{
    margin: auto;
}
.graficas{
    display: flex;
    width: 100%;
    height: 300px;
    padding: 20px;
}
.graficas .grafica{
    margin: auto;
    width: 500px;
}
.graficas .info{
    margin: auto;
    text-align: justify;
    padding-left: 50px;
}

.modulos{
    display:inline-flex;
    width: 100%;
    padding: 20px;
}
.modulos .tarjetaModulo{
    padding: 20px;
}

</style>