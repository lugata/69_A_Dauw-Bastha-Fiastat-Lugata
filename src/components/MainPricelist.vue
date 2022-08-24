<template>
<section v-for="data in daftar"> 
    <div class="container">
        <div class="row p-5 " >
            <div class="col-12 text-center" >
                <h1 class="fw-bolder">{{data.judul}}</h1>
            <div class="pt-5 position-relative top-50 start-50 translate-middle">
                <img :src="data.foto" alt="" class="gambar"/>
            </div>
            </div>
        </div>

        <div class="row p-5" id="rtext">

            <div class="col-4"></div>
            <div class="col-4 text-center">
            <p> <strong>{{data.bdeskripsi}}</strong> {{data.deskripsi}}</p>
            </div>
            <div class="col-4"></div>

        </div>

<ol>
        <div class="row py-1 px-5 justify-content-md-center">
            <div class="col-1" style="color:transparent;"><li></li></div>
            <div class="col-2"></div>
            <div class="col-2 fw-bolder fs-4">{{data.jenis1}}</div>
            <div class="col-2"></div>
            <div class="col-1"></div>
            <div class="col-2 fw-bolder fs-4">{{data.jenis2}}</div>
            <div class="col-2"></div>
        </div>
</ol>
<ol>
        <div class="row py-2 px-5 justify-content-md-center fw-bold">
            <div class="col-1" style="color:transparent;"><li></li></div>
            <div class="col-2">Ukuran</div>
            <div class="col-2">{{data.menulist}}</div>
            <div class="col-2">Harga</div>
            <div class="col-1"></div>
            <div class="col-2">{{data.menulist}}</div>
            <div class="col-2">Harga</div>

        </div> 
</ol>
<ol type="1">
    <div class="list" v-for="lisst in data.daftar">
            <div class="row py-3 px-5 justify-content-md-center fw-bold">
                <div class="col-1"><li></li></div>
                <div class="col-2" v-for="(baris1, $index) in lisst.paket1">{{baris1}}</div>
                <div class="col-1"></div>
                <div class="col-2" v-for="(kanan1, $index) in lisst.bagian1">{{kanan1}}</div>
            </div> 
            <div class="row py-3 px-5 justify-content-md-center fw-bold">
                <div class="col-1"><li></li></div>
                <div class="col-2" v-for="(baris2, $index) in lisst.paket2">{{baris2}}</div>
                <div class="col-1"></div>
                <div class="col-2" v-for="(kanan2, $index) in lisst.bagian2">{{kanan2}}</div>
            </div>
            <div class="row py-3 px-5 justify-content-md-center fw-bold">
                <div class="col-1"><li></li></div>
                <div class="col-2" v-for="(baris3, $index) in lisst.paket3">{{baris3}}</div>
                <div class="col-1"></div>
                <div class="col-2" v-for="(kanan3, $index) in lisst.bagian3">{{kanan3}}</div>
            </div> 
            <div class="row py-3 px-5 justify-content-md-center fw-bold">
                <div class="col-1"><li></li></div>
                <div class="col-2" v-for="(baris4, $index) in lisst.paket4">{{baris4}}</div>
                <div class="col-1"></div>
                <div class="col-2" v-for="(kanan4, $index) in lisst.bagian4">{{kanan4}}</div>
            </div>
            <div class="row py-3 px-5 justify-content-md-center fw-bold">
                <div class="col-1"><li></li></div>
                <div class="col-2" v-for="(baris5, $index) in lisst.paket5">{{baris5}}</div>
                <div class="col-1"></div>
                <div class="col-2" v-for="(kanan5, $index) in lisst.bagian5">{{kanan5}}</div>
            </div> 
            <div class="row py-3 px-5 justify-content-md-center fw-bold">
                <div class="col-1"><li></li></div>
                <div class="col-2" v-for="(baris6, $index) in lisst.paket6">{{baris6}}</div>
                <div class="col-1"></div>
                <div class="col-2" v-for="(kanan6, $index) in lisst.bagian6">{{kanan6}}</div>
            </div>
            <div class="row py-3 px-5 justify-content-md-center fw-bold">
                <div class="col-1"><li></li></div>
                <div class="col-2" v-for="(baris7, $index) in lisst.paket7">{{baris7}}</div>
                <div class="col-1"></div>
                <div class="col-2" v-for="(kanan7, $index) in lisst.bagian7">{{kanan7}}</div>
            </div>
        </div>
</ol> 
</div>
</section>
</template>


<script>

export default{
    name: "MainPricelist",
    props: {

    },
    data() {
        return {
            daftar:[],
        }
    },
    mounted(){
        fetch('/assets/Data/data.json')
        .then(response => response.json())
        .then(response => {
            this.daftar = response.data
        })
        .catch(err => console.log(err.message))
    }
}
</script>

<style>
.gambar{
    width: 100vh;
    height: auto;
}
</style>