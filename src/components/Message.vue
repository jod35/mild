<template>
    <div class="messages">
        <div class="message" v-for="message in messages" :key="message.id">
            <p>{{message.text}} <br> for the {{message.id}} time</p>
        </div>
    </div>
</template>

<script>
export default {
    name:"Message",
    props:["messages"]
}
</script>
<style>
.messages{
    margin-top: 50px;
}
.messages > .message +.message{
    margin-top: 20px;
}
.message{
    padding: 20px;
    color: white;
    background-color: rgb(117, 143, 79);
}
</style>