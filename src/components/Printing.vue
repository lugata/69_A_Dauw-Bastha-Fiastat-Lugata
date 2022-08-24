<template>

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

            <div class="mainloop" v-for="(mjenis, index) in mjenis">

                    <div class="row" > 
                        <div class="col-12 pt-5 text-center" >
                            <img src="/assets/PDesign.png" alt="" class="gambar"/>
                            <p class="fw-bold mt-4 fs-4">{{mjenis.jenis}}</p>
                        </div>
                    </div>



                    <div class="row p-3 " id="rtext" >
                        <div class="loop col-4 g-5" v-for="(items, index) in items">
                        <div class="list" >
                        <p class="text-center" id="ntext">{{ index+1 }}</p>   
                        <p>{{ items.message }}</p> </div>
                        </div>
                    </div> 



                    </div>
                    
            </div>
        
</template>

<script>
export default{
    data(){
        return {
            items: [{ message: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna'}, 
            { message: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna'},
            { message: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna'},
            { message: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna'},
            { message: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna'},
            { message: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna'}
            ],
            mjenis: [{ jenis: 'SURELAB PRINTING'}, { jenis: 'BASIC PRINTING'}]
        }
    },
    name: "Printing",
    props: {
        judul: String,
       
    },


}
</script>

<style>
.gambar{
    max-width: 100%;
    height: auto;
}

</style>