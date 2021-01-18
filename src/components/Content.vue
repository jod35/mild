<template>
    <div class="container">
        {{message}}
        <p class="count">
            The button below has been clicked {{messages.length}} times
        </p>
        <input type="text" v-model="text" placeholder="Your Text">
        <button  @click="addCount">Add Count</button>
        <button @click="clearAll">Clear Item</button>
        <Message :messages="messages"/>
    </div>
</template>
<script>

import Message from './Message.vue'


export default {
    name:"Content",
    components:{
        Message
    },
    props:["message","name"],
    data(){
        return{
            count:0,
            messages:[],
            text:""
        }
    },
    methods:{
        addCount(){
            this.count ++;
            this.messages.push({ "id":this.count,
                                    "text":this.text
                                    });
            console.log(this.messages);
        },
        clearAll(){
            this.messages.shift()
            this.count --;
        }
    }
}
</script>
<style>
    .container{
        width: 80%;
        padding: 5%;
    }
    .count{
        font-size: 2em;
    }
</style>