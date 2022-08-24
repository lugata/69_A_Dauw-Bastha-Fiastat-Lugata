<template>
    <MyNav logo="LOGO"/>
    <Printing
        judul="Printing" 
    />
    <MyFooter/>
</template>


<script>
import MyNav from '@/components/MyNav.vue'
import Printing from '@/components/Printing.vue'
import MyFooter from '@/components/MyFooter.vue'


export default {
  name: 'printing',
  components: {
    MyNav,
    Printing,
    MyFooter,
    
}
}
</script>