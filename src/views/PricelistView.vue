<template>
<MyNav logo="LOGO"/>
<Pricelist tanggal="Juli 2022"/>
<MainPricelist 
  judul="Photography" 
  jenis="JENIS" 
  jenis2="JENIS2"
  menu1="Per-Foto"
  menu2="Harga" 
  no="1"
  ukuran="4x6"
  foto="1"
  harga="Rp. 100.000"
  foto2="2"
  harga2="Rp. 50.000"/>
  <MyFooter/>
</template>

<script>
// @ is an alias to /src
import MyNav from '@/components/MyNav.vue'
import Pricelist from '@/components/Pricelist.vue'
import MainPricelist from '@/components/MainPricelist.vue'
import MyFooter from '@/components/MyFooter.vue'


export default {
  name: 'PricelistView',
  components: {
    MyNav,
    Pricelist,
    MainPricelist,
    MyFooter
}
}
</script>