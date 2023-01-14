<template>
    <div>
    <div class="container-fluid">
    <div class="row gap-5 mx-3 d-sm-flex justify-content-center">
            <div class="card" v-for="item in testimonials" :key="item">
                <img :src="item.image" 
                style="width: 15rem;"/>
                <div class="card-body">
                    <h5 class="card-title">{{ item.name }}</h5>
                    <p class="card-text">{{ item.relationship }}</p>
                    <p class="testimony">{{ item.testimony}}</p>
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
        testimonials:[
            {
            name: "Kelebogile Nobomvu",
            image:"https://i.postimg.cc/bw1qghhH/Lebo.jpg",
            relationship:"Collegue",
            testimony: "Buhle is a sweet and loving soul. She is a hard worker and once she puts her mind to something she get it done."
            },
            {
            name: "Candice Amon",
            image:"https://i.postimg.cc/7Y8H2hvY/Candice.jpg",
            relationship:"Facilitator",
            testimony: "Buhle is a very kind hearted person.Always ready to extend a helping hand and also knows when to ask for help. She believes in being a positive role model to those who look up to her and carries herself very well. A key value she holds dear is Respect."
            },
            {
            name: "Thokozani Nqwili",
            image:'https://i.postimg.cc/7PQ78gTt/Thoko.jpg',
            relationship:"Collegue",
            testimony: "Buhle is a very dedicated individual with a positive mind set. She works well with people and she has the ability to think out of the box."
            },
            {
            name: "Sibabalwe Mafestire",
            image:'https://i.postimg.cc/XvzGSWrG/Siba.jpg',
            relationship:"Collegue",
            testimony: "Buhle is a dedicated individual who puts her all in her work and a good team player, good at planning and meeting deadlines"
            },
            {
            name: "Sindile Kula",
            image:"https://i.postimg.cc/Dwm7VXL6/Sindile.jpg",
            relationship:"Collegue",
            testimony:"Buhle is a bright young lady who is incredibly ambitious and laser-focused on her life goals.She has a fantastic memory and picks things up really quickly.She is a person who puts a lot of effort into whatever she does and tries her absolute best." 
            },
            {
            name:"Sakhe Mzolisa",
            image:"https://i.postimg.cc/dVz34Bpr/Sakhe.jpg",
            relationship: "Collegue",
            testimony:"Change is what drives Buhle. She is a go-getter who is committed to her work. She always looking forward in upskilling and developing her skills. A person who can mitigate between risks. A great advocate for honesty, assertiveness and resilience. She has a bubbly personality and is always willing to land a helping hand hence her nickname 'Bubbles'. A real asset to any environment she is in."
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
@media screen and (max-width: 720px) {
    .card {
        width: 20rem;
    }
}

@media screen and (max-width:630px) {
    .card {
        width: 20rem;
    }
}


@media screen and (max-width: 300px)
{
    .card {
        width: 10rem;
    }
}
</style>