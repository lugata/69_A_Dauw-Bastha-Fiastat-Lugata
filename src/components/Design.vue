<template>
        <section> 
        <div class="container">
        <div class="row p-5 ">
            <div class="col-12 text-center ">
                <h1 class="fw-bolder ">{{judul}}</h1>
            <div class="pt-3 pb-4 position-relative top-50 start-50 translate-middle">
                <img src="/assets/PDesign.png" alt="" class="gambar"/>
            </div>
            </div>         

        </div>
        
        <div class="row p-3" id="rtext">

            <div class="col-1 col-md-4"></div>
            <div class="col-10 col-md-4 text-center">
            <p><strong>Lorem ipsum </strong> dolor sit amet, consectetur. ullamcorper tellus id nibh urna. Fermentum ullamcorper tellus id nibh urna. Faucibus tellus facilisis molestie amet nisl.</p>
            </div>
            <div class="col-1 col-md-4"></div>

        </div>

        <div class="row"> 
            <div class="col-6 text-center">
                <img src="/assets/PDesign.png" alt="" class="gambar"/>
                <p class="fw-bold mt-4">CREATIVE</p>
            </div>
            <div class="col-6 text-center">
                <img src="/assets/PDesign.png" alt="" class="gambar"/>
                <p class="fw-bold mt-4">BASIC</p>
            </div>
        </div>

        <div class="row mt-5"> 
            <div class="col-6 text-left">
                <p class="fw-bold fs-5 mt-4">NOTE :</p>
            </div>
            <div class="col-6 text-left">

            </div>
        </div>

        <ol type="1">
        <div class="row  p-3" id="rtext">
            
                    <li class="fw-2 col-6 col-md-4" v-for="i in 6" :key="i">
                        <p>Lorem ipsum dolor sit amet, consectetur. ullamcorper tellus id nibh urna. Fermentum ullamcorper tellus id nibh urna. Faucibus tellus facilisis molestie amet nisl.</p>
                    </li>

        </div>
        </ol>

        </div>
        

        </section>
</template>

<script>
export default{
    name: "Design",
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