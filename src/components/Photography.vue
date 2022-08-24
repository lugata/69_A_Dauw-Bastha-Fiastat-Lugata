<template>
        <section> 
        <div class="container">
        <div class="row p-5 ">
            <div class="col-12 text-center ">
                <h1 class="fw-bolder ">{{judul}}</h1>
            <div class="pt-3 pb-4 position-relative top-50 start-50 translate-middle">
                <img src="/assets/photography.png" alt="" class="gambar"/>
            </div>
            </div>         

        </div>
        
        <div class="row p-3" id="rtext">

            <div class="col-3 col-md-4"></div>
            <div class="col-6 col-md-4 text-center">
            <p><strong>Lorem ipsum </strong> dolor sit amet, consectetur. ullamcorper tellus id nibh urna. Fermentum ullamcorper tellus id nibh urna. Faucibus tellus facilisis molestie amet nisl.</p>
            </div>
            <div class="col-3 col-md-4"></div>

        </div>

        <div class="row"> 
            <div class="col-6 text-center">
                <img src="/assets/photography.png" alt="" class="gambar"/>
                <p class="fw-bold mt-4">FORMAL</p>
            </div>
            <div class="col-6 text-center">
                <img src="/assets/photography.png" alt="" class="gambar"/>
                <p class="fw-bold mt-4">UNFORMAL</p>
            </div>
        </div>

        <div class="row p-3" id="rtext">

            <div class="col-3 col-md-4"></div>
            <div class="col-6 col-md-4 text-center">
            <p><strong>Lorem ipsum </strong> dolor sit amet, consectetur. ullamcorper tellus id nibh urna. Fermentum ullamcorper tellus id nibh urna. Faucibus tellus facilisis molestie amet nisl.</p>
            </div>
            <div class="col-3 col-md-4"></div>

        </div>
        </div>
        

        </section>
</template>

<script>
export default{
    name: "Photography",
    props: {
        judul: String,
       
    }
}
</script>

<style>
.gambar{
    max-width: 100%;
    height: auto;
}
</style>