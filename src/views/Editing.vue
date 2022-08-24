<template>
    <MyNav logo="LOGO"/>
    <Editing
        judul="Editing" 
    />
    <MyFooter/>
</template>


<script>
import MyNav from '@/components/MyNav.vue'
import Editing from '@/components/Editing.vue'
import MyFooter from '@/components/MyFooter.vue'

export default {
  name: 'editing',
  components: {
    MyNav,
    Editing,
    MyFooter,
    
}
}
</script>