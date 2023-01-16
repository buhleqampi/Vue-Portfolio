<template>
        <form action="https://formspree.io/f/{form_id}" method="post">
            <div class="mb-3">
            <label for="exampleInputname" class="form-label">Full Name</label>
            <input type="name" class="form-control" id="exampleInputName1" aria-describedby="nameHelp" placeholder="Insert your full name..." required>
            </div>
            <label for="exampleInputEmail1" class="form-label">Email address</label>
            <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="Your email address..." required>
            <div class="mb-3">
            <label for="exampleInputPassword1" class="form-label">Password</label>
            <input type="password" class="form-control" id="exampleInputPassword1" placeholder="password" required>
            </div>
            <button v-on:click.prevent="display" >Submit</button>
        </form>
</template>
<script>
export default {
    methods: {
        display() {
            alert("Are you sure you want to submit this?");
        }    
    }
}
</script>

<style scoped>
div {
    box-shadow: 5px solid orange;
}
form input{
    margin:10px;
    width: 50%;
} 
</style>