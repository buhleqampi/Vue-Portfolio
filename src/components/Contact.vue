<template>
    <div class="container px-5">
        <div class="row" style="height: 100%;">
        <h2 class="d-flex justify-content-center mt-5 text-white">Contact me</h2>
    <form target="_blank" action="https://formspree.io/f/xqknwllo" method="POST">
        <div class="row mt-4">
        <div class="col-lg-6 my-3 shadow">
            <input required type="text" name="name" class="form-control bg-white text-white" id="name"
            placeholder="Name" style="height: 50px;">
        </div>
        <div class="col-lg-6 my-3 shadow">
            <input required type="email" name="email" class="form-control bg-white text-white" id="email"
            placeholder="Email" style="height: 50px;">
        </div>
        <div class="mt-4 shadow">
            <textarea id="message" class="form-control bg-white text-white"
            placeholder="Tell us more about your needs...." style="height: 200px;"></textarea>
        </div>
        <div class="my-4 text-center">
            <button type="submit" class="btn btn-lg btn-danger btn-outline-secondary rounded-pill">Send
            message</button>
        </div>
        </div>
    </form>
    
        <div class="row mt-5">
        <div class="col-lg-4 my-2">
            <h4 class="text-white my-4">Address</h4>
            <div class="row text-light mt-4">
            <div class="icon text-danger">
                <i class="fa-solid fa-location-dot"></i>
            </div>
            <p>22 Jacob Street</p>
            <p>Nyanga</p>
            <p>7750</p>
            </div>
        </div>
        <div class="row mt-4">
            <div class="phone d-flex flex-row">
            <div class="icon text-danger">
                <i class="fa-solid fa-phone"></i>
            </div>
            <p class="text-light ms-3">(065) 559 8353</p>
            </div>
            <div class="mobile d-flex flex-row">
            <div class="icon text-danger">
                <i class="fa-solid fa-mobile"></i>
            </div>
            <p class="text-light ms-3">(063) 063 0263</p>
            </div>
            <div class="email d-flex flex-row">
            <div class="icon text-danger">
                <i class="fa-solid fa-envelope"></i>
            </div>
            <p class="text-light ms-3">buhle3857@gmail.com</p>
            </div>
        </div>
        </div>
        </div>
        </div>
        
</template>

<style scoped>
div {
    box-shadow: 5px solid orange;
}
form input{
    margin:10px;
    width: 50%;
} 
</style>