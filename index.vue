<script>
import NavBar from '../components/NavBar.vue';
import Footer from '../components/Footer.vue';
import Content from '../components/Content.vue';


  export default{
    layout: "custom",
    components: { NavBar, Footer, Content }
}
</script>
<template>
 <div>
   <NavBar/>
   <moreHero/>
   <Content/>
   <Footer/>
 </div>
</template>
