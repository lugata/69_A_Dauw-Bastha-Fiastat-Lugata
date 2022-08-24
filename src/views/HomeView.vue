<template>
<MyNav logo="LOGO"/>
<HomeMain vjudul1="Andal Studio"/>
<MyFooter/>
</template>

<script>
// @ is an alias to /src
import MyNav from '@/components/MyNav.vue'
import HomeMain from '@/components/HomeMain.vue'
import MyFooter from '@/components/MyFooter.vue'


export default {
  name: 'HomeView',
  components: {
    MyNav,
    HomeMain,
    MyFooter
}
}
</script>
