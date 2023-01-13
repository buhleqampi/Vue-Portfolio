<template>
        <h4 class="d-flex justify-content-center mt-5 p-5 text-white pb-10"> My skills</h4>
        <div class="row mt-3">
        <h4 class="text-white"></h4>
        <div class="col-lg-6">
            <div class="languages d-flex">
            <p class="text-light mt-3">HTML</p>
            <p class="text-light mt-3">95%</p>
            </div>
            <div class="progress" style="height: 10px;">
            <div class="progress-bar bg-danger" role="progressbar" style="width: 95%" aria-valuenow="95"
                aria-valuemin="0" aria-valuemax="100"></div>
            </div>
            <div class="languages d-flex">
            <p class="text-light mt-3">CSS</p>
            <p class="text-light mt-3">70%</p>
            </div>
            <div class="progress" style="height: 10px;">
            <div class="progress-bar bg-danger" role="progressbar" style="width: 70%" aria-valuenow="70"
                aria-valuemin="0" aria-valuemax="100"></div>
            </div>
            <div class="languages d-flex">
            <p class="text-light mt-3">Bootstrap</p>
            <p class="text-light mt-3">80%</p>
            </div>
            <div class="progress mb-5" style="height: 10px;">
            <div class="progress-bar bg-danger" role="progressbar" style="width: 80%" aria-valuenow="80"
                aria-valuemin="0" aria-valuemax="100"></div>
            </div>
        </div>
        <div class="col-lg-6">
            <div class="languages d-flex">
            <p class="text-light mt-3">JavaScript</p>
            <p class="text-light mt-3">5%</p>
            </div>
            <div class="progress" style="height: 10px;">
            <div class="progress-bar bg-danger" role="progressbar" style="width: 5%" aria-valuenow="5" aria-valuemin="0"
                aria-valuemax="100"></div>
            </div>
            <div class="languages d-flex">
            <p class="text-light mt-3">Python</p>
            <p class="text-light mt-3">5%</p>
            </div>
            <div class="progress" style="height: 10px;">
            <div class="progress-bar bg-danger" role="progressbar" style="width: 5%" aria-valuenow="5" aria-valuemin="0"
                aria-valuemax="100"></div>
            </div>
            <div class="languages d-flex">
            <p class="text-light mt-3">Microsoft Office</p>
            <p class="text-light mt-3">100%</p>
            </div>
            <div class="progress mb-5" style="height: 10px;">
            <div class="progress-bar bg-danger" role="progressbar" style="width: 100%" aria-valuenow="100"
                aria-valuemin="0" aria-valuemax="100"></div>
            </div>
        </div>
        <div class="mb-4 text-center">
            <a href="./Assets/Buhle Qampi CV.pdf" download="">
            <button type="button" class="btn btn-outline-secondary btn-lg rounded-pill">Download CV <i
                class="fa-solid fa-download"></i></button>
            </a>
        </div>
        </div>


    <div class="col-2" v-for="item in projects" :key="item">
        <div>
        <div class="card">
            <img :src="item.image" 
            style="width: 30rem;margin-left:3rem" 
            />
            <div class="card-body">
                <h5 class="card-title">{{ item.name }}</h5>
                <p class="card-text">{{ item.description }}</p>
                <button class="btn btn-primary">{{ item.github}}</button>
                <button class="btn btn-primary">{{ item.netlify}}</button>
            </div>
        </div>
    </div>
    </div>
</template>
<script>
export default {
    data () {
        return {
            projects: [
                {
                name: "HTML/CSS Portfolio",
                description:"This was my first project in the form of a personal portfolio. I used HTML and CSS.",
                GitHub:"",
                Netlify:""
                },
                {name: "Netflix website",
                description:"This was my first project in HTML and CSS.",
                GitHub:"",
                Netlify:""
                },
                {name: "E-commerce website",
                description:"E-commerce I used HTML and CSS.",
                GitHub:"https://github.com/buhleqampi/Ecommerce.git",
                Netlify:"https://buhleqampi-ecommerce-site.netlify.app/"
                },
                {
                name: "JS Calculator",
                description:"E-commerce I used HTML and CSS.",
                GitHub:"",
                Netlify:""
                },
                {
                name: "Point of Sale",
                description:"Lorem ggggggggggg.",
                GitHub:"",
                Netlify:"" 
                }
            ]
        }
    }
    
}
</script>
<style lang="">
    
</style>