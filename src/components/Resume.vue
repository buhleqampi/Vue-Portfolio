<template>
    <div class="container px-5">
        <div class="row" style="height: 100%;">
        <h2 class="d-flex justify-content-center mt-5 text-white">Resume</h2>
    <div>
    <div class="container-fluid">
    <div class="row gap-5 mx-3 d-sm-flex justify-content-center">
    <div class="card" v-for="item in skills" :key="item">
            <img :src="item.image" class="mx-auto d-block" style="width: 15rem;" />
            <div class="card-body">
                <h5 class="card-title">{{ item.name }}</h5>
                <p class="card-text">{{ item.progress }}</p>
            </div>
        </div>
    </div>
    </div>
</div>
</div>
</div>
</template>

<script>

export default {
data () {
    return {
        skills:[
            {
            name: "HTML",
            image:"https://i.postimg.cc/VksC4C9R/png-clipart-html-5-logo-web-development-html-css3-canvas-element-web-design-w3c-html5-logo-miscellan.png",
            progress:"90%",
            },
            {
            name: "CSS",
            image:"https://i.postimg.cc/SK6bsJ5B/css-318-698167.webp",
            progress:"70%"
            },
            {
            name: "Bootstrap",
            image:'https://i.postimg.cc/cC5VjYgn/bootstrap-icons.png',
            progress:"80%"
            },
            {
            name: "JavaScript",
            image:'https://i.postimg.cc/Hk068XY9/Javascript-Logo.png',
            progress:"60%"
            },
            {
            name: "Vue.js",
            image:"https://i.postimg.cc/4xGr0Jnw/logo.png",
            progress:"60%",
            },
            {
            name:"Python",
            image:"https://i.postimg.cc/N0zCQYG3/5968350.png",
            progress: "5%",
            }
        ]
    }
}
} 
</script>

<style scoped>
.card {
    box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
    transition: 0.3s;
    width: 20rem;
}
.card:hover {
    box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);  
}
.card-body {
    padding: 2px 16px;
}

</style>