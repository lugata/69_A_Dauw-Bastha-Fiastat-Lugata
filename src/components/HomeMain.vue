<template>

    <section class="hal1 mb-5">
        <div class="container-fluid mt-5">
            <div class="d-grid gap-5">
                <div class="motto">              
                    <div class="text-center" id="rtext">
                        <p class="fs-2 fw-normal" style="margin-bottom: -1px;">Andal Studio</p>
                    </div>
                    <div class="text-center" id="btext">
                        <p class="moto fw-bold">THAT'S PROFESSIONAL <br> WILL DO!</p>
                    </div>
                </div>
            </div>
        </div>                  
    </section>

    <div class="intro">
        <h1>{{vjudul1}}</h1>
        <video src="/assets/Sequence 01.mp4"></video>
      </div>
 <section class="hal2">
        <div class="container">        
            <div class="text-center" >
            <p class="fs-4 fw-normal" id="rtext" style="margin-bottom: 100px;"><strong id="btext">Our company</strong> is dedicated to providing <br> creative professional services of <br> the highest quality.</p>
            </div>
            <div class="product">
                <div class="d-grid gap-4">
                    <div class="row">
                        <div class="col-12" id="cardhal2" >
                            <div class="card text-black" id="cards">
                                <img src="/assets/Photography.png" class="card-img"  alt="..."/>
                                <div class="card-img-overlay">
                                  <h1 class="card-title mx-4 mt-4" id="btext" style="font-weight: 600; font-size: 60px;">Photography</h1>
                                  <router-link to = "/photography" id="btnhal2" class="btn btn-outline-dark rounded-pill px-4 py-3 mx-4 mt-2 fs-5">Learn more</router-link>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="row">
                        <div class="col-12 col-xl-6 mb-4" >
                        <router-link to = "/editing"><div class="card text-black" id="cards">
                                <img src="/assets/Editing.png" class="card-img" alt="..." />
                                <div class="card-img-overlay">
                                  <h1 class="card-title mx-4 mt-4" id="btext" style="font-weight: 600; font-size: 60px;">Editing</h1>
                                </div>
                            </div> </router-link>
                        </div>
                        <div class="col-12 col-xl-6" >
                        <router-link to="/design"><div class="card text-black" id="cards">
                                <img src="/assets/Design.png" class="card-img" alt="..." />
                                <div class="card-img-overlay">
                                  <h1 class="card-title mx-4 mt-4" id="btext" style="font-weight: 600; font-size: 60px;">Design</h1>
                                </div>
                            </div> </router-link>
                        </div> 
                    </div>
                    
                    <div class="row">
                        <div class="col-12" id="cardhal2" >
                            <div class="card text-black" id="cards">
                                <img src="/assets/Printing.png" class="card-img" alt="..." />
                                <div class="card-img-overlay">
                                  <h1 class="card-title mx-4 mt-4" id="btext" style="font-weight: 600; font-size: 60px;">Printing</h1>
                                  <router-link to = "/printing" id="btnhal2" class="btn btn-outline-dark rounded-pill px-4 py-3 mx-4 mt-2 fs-5">Learn more</router-link>
                                </div>
                            </div>
                        </div>
                    </div>

                </div>
            </div>
        </div>
    </section>

    <section class="Delivery" style="margin: 100px 0;">
        <div class="container">
            <div class="text-left" >
                <p class="mb-4" id="btext" style="margin-bottom: 100px; font-weight: 600; font-size: 60px;">Delivery</p>
                </div>
            <div class="row">
                <div class="col-5" id="rtext" style="font-size: 18px;">
                    <p>We deliver our products worldwide. Delivery costs depend on batch size and are determined with the supplier beforehand. Our products are always delivered in whichever way is most accessible and beneficial for you.</p>
                </div>  
                <div class="col-7">
                </div>  
            </div> 
            <div class="row mt-5">
                <div class="col-12 col-md-4">
                    <img src="assets/Truck.png" id="fotdelivery" class="card-img" alt="..." >

                      <p class="fw-bold fs-5">Darat</p>
                      <p>We deliver our products worldwide. Delivery costs depend on batch size and are determined with the supplier beforehand. Our products are always delivered in whichever way is most accessible and beneficial for you.</p>
 
                  </div>  
                <div class="col-12 col-md-4">
                    <img src="assets/Kapal Laut.png" id="fotdelivery" class="card-img" alt="...">

                      <p class="fw-bold fs-5">Laut</p>
                      <p>We deliver our products worldwide. Delivery costs depend on batch size and are determined with the supplier beforehand. Our products are always delivered in whichever way is most accessible and beneficial for you.</p>
                </div>  
                <div class="col-12 col-md-4">
                    <img src="assets/COD.png" id="fotdelivery" class="card-img" alt="...">

                      <p class="fw-bold fs-5">Pickup</p>
                      <p>We deliver our products worldwide. Delivery costs depend on batch size and are determined with the supplier beforehand. Our products are always delivered in whichever way is most accessible and beneficial for you.</p>
                  </div>  
            </div>        
      </div>  
       
    </section>

</template>  


<script>


export default {
  name: 'HomeMain',
  props: {
    vjudul1: String,
    logo: String,
    
  }
}


</script>


<style>

#cards{
    transition: all 0.2s ease;
}

#cards:hover{

    box-shadow: 5px 6px 6px 2px #e9ecef;
    transform: scale(1.02);
}

.moto{
    font-size: 3em;
  }

  .hal1{  

    overflow: hidden;
  }

  .intro {
    height: 100vh;
  }
  
  .intro video {
    height: 100%;
    width: 100%;
    object-fit: cover;
  }
  
  .intro h1 {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    font-size: 80px;
    color: var(--main);
  }

 .hal2{ 
    margin: 100px 0;
 }

 #cardhal2{
  transition: 0.5s;
 }



 #btnhal2{

    border: 2px solid var(--bgbtn); 
    color:var(--secondary); 
    transition: 0.5s; 
  
 }

 #btnhal2:hover{
  color: var(--white); 
  background: var(--secondary); 
 }






</style>