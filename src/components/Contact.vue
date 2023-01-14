<template>
        <form action="https://formspree.io/f/{form_id}" method="post">
            <div class="mb-3">
            <label for="exampleInputEmail1" class="form-label">Full Name</label>
            <input type="name" class="form-control" id="exampleInputName1" aria-describedby="nameHelp">
            <div id="nameHelp" class="form-text">We'll never share your email with anyone else.</div>
            </div>
            <label for="exampleInputEmail1" class="form-label">Email address</label>
            <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp">
            <div id="emailHelp" class="form-text">We'll never share your email with anyone else.</div>
            <div class="mb-3">
            <label for="exampleInputPassword1" class="form-label">Password</label>
            <input type="password" class="form-control" id="exampleInputPassword1">
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
</script>
.form {

}
<style scoped>
    
</style>