<template>
<div class="container">
    <div>
    <div class="col-2" v-for="item in skills" :key="item">
    <div>
    <div class="card">
        <img :src="item.image" 
        style="width: 15em;align-items: center" 
        />
        <div class="card-body">
            <h5 class="card-title">{{ item.name }}</h5>
            <p class="card-text">{{ item.progress }}</p>
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