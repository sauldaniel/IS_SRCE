<template>
    <div class="tarjetaModulo">

        

            <div class="card" style="width: 18rem;">
                    <img :src="rutaIMG" class="card-img-top">
                    
                <div class="card-body">
                    <h5 class="card-title">{{moduleName}}</h5>
                    <p class="card-text">{{ moduleDescription }}</p>
                    <a :href="redirect" class="btn btn-primary">Ir</a>
                </div>
            </div>
        
        
    </div>
</template>

<script>

export default {
  name: 'tarjetaModulo',
  props: {
    moduleName: String,
    moduleDescription: String,
    redirect: String,
    rutaIMG: String
  }
}

</script>

<style>

.card img{
  width: 100%;
  height: 150px;
}

.card h5{
  height: 50px;
}
.card p{
  height: 80px;
  text-align: justify;
}
.card a{
  width: 80px;
}
</style>