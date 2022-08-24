<template>

<div class="row p-5" id="hal1">
    <div class="col-12 text-center">
        <h1 class="fw-bolder">PriceList</h1>
        <p class="fw-bold">dated as {{tanggal}}</p>
        <img src="/assets/Pricelist.png" alt="" class="pheader"/>
    </div>
</div>

</template>

<script>


export default {
  name: 'PriceList',
  props: {
    tanggal: String,

  }
  
}


</script>

<style>


#hal1 {
    background: var(--bgbtn);
    height: 600px;
  display: flex;
  align-items: center;
  justify-content: center;
  
}

.pheader{
  max-width: 600px;

}




</style>