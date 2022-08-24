<template>
    <MyNav logo="LOGO"/>
    <Design judul="Design"/>
    <MyFooter/>
</template>


<script>
import MyNav from '@/components/MyNav.vue'
import Design from '@/components/Design.vue'
import MyFooter from '@/components/MyFooter.vue'



export default {
  name: 'design',
  components: {
    MyNav,
    Design,
    MyFooter,

}
}
</script>