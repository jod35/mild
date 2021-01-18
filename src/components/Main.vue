<template>
    <div class="main">
        <SideBar/>
        <Content :message="message"/>
        
    </div>
</template>
<script>
import SideBar from './SideBar.vue'
import Content from './Content.vue'
export default {
    name:"Main",
    components:{
        SideBar,
        Content
    },
    data(){
        return{
            message:"This is the right side"
        }
    }
    
}
</script>
<style>
 .main{
     min-height: 100vh;
     position: relative;
     top: 70px;
     display: flex;
 }
</style>