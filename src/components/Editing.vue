<template>
        <section> 
        <div class="container">
        <div class="row p-5 ">
            <div class="col-12 text-center ">
                <h1 class="fw-bolder ">{{judul}}</h1>
            <div class="pt-3 pb-4 position-relative top-50 start-50 translate-middle">
                <img src="/assets/PEditing.png" alt="" class="gambar"/>
            </div>
            </div>         

        </div>
        
        <div class="row p-3" id="rtext">

            <div class="col-4"></div>
            <div class="col-4 text-center">
            <p><strong>Lorem ipsum </strong> dolor sit amet, consectetur. ullamcorper tellus id nibh urna. Fermentum ullamcorper tellus id nibh urna. Faucibus tellus facilisis molestie amet nisl.</p>
            </div>
            <div class="col-4"></div>

        </div>

        <div class="row mt-5"> 
            <div class="col-6 text-left">
                <p class="fw-bold fs-5 mt-4">NOTE :</p>
            </div>
            <div class="col-6 text-left">

            </div>
        </div>

        <ol type="1">
        <div class="row p-3" id="rtext">
            
                <div class="col-4">
                    <li class="fw-2">
                        <p>Lorem ipsum dolor sit amet, consectetur. ullamcorper tellus id nibh urna. Fermentum ullamcorper tellus id nibh urna. Faucibus tellus facilisis molestie amet nisl.</p>
                    </li>
                </div>
                <div class="col-4">
                
                    <li class="fw-2">
                        <p>Lorem ipsum dolor sit amet, consectetur. ullamcorper tellus id nibh urna. Fermentum ullamcorper tellus id nibh urna. Faucibus tellus facilisis molestie amet nisl.</p>
                    </li>
        
                </div>
                <div class="col-4">
                    <li class="fw-2">
                        <p>Lorem ipsum dolor sit amet, consectetur. ullamcorper tellus id nibh urna. Fermentum ullamcorper tellus id nibh urna. Faucibus tellus facilisis molestie amet nisl.</p>
                    </li>
                </div>
            
        </div>
        <div class="row p-3" id="rtext">
            
                <div class="col-4">
                    <li class="fw-2">
                        <p>Lorem ipsum dolor sit amet, consectetur. ullamcorper tellus id nibh urna. Fermentum ullamcorper tellus id nibh urna. Faucibus tellus facilisis molestie amet nisl.</p>
                    </li>
                </div>
                <div class="col-4">
                
                    <li class="fw-2">
                        <p>Lorem ipsum dolor sit amet, consectetur. ullamcorper tellus id nibh urna. Fermentum ullamcorper tellus id nibh urna. Faucibus tellus facilisis molestie amet nisl.</p>
                    </li>
        
                </div>
                <div class="col-4">
                    <li class="fw-2">
                        <p>Lorem ipsum dolor sit amet, consectetur. ullamcorper tellus id nibh urna. Fermentum ullamcorper tellus id nibh urna. Faucibus tellus facilisis molestie amet nisl.</p>
                    </li>
                </div>
            
        </div>
        </ol>

        </div>
        

        </section>
</template>

<script>
export default{
    name: "Editing",
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