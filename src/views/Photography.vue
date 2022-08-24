<template>
<MyNav logo="LOGO"/>
<Photography
    judul="Photography" 
/>
<MyFooter/>
</template>


<script>
import MyNav from '@/components/MyNav.vue'
import Photography from '@/components/Photography.vue'
import MyFooter from '@/components/MyFooter.vue'

export default {
  name: 'photography',
  components: {
    MyNav,
    Photography,
    MyFooter
}
}
</script>