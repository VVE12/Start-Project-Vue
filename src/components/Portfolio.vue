<template>
    <section class="bg-light" id="portfolio">
        <div class="container">
            <div class="row">
                <div class="col-lg-12 text-center">
                    <h2 class="section-heading text-uppercase">Portfolio</h2>
                    <h3 class="section-subheading text-muted">Lorem ipsum dolor sit amet consectetur.</h3>
                </div>
            </div>
        <div class="row">
            <div class="col-md-4 col-sm-6 portfolio-item" v-for="(obj, key) in portfolioJSON" :key="key">
                <a class="portfolio-link" data-toggle="modal" href="#portfolioModal2">
                    <div class="portfolio-hover">
                        <div class="portfolio-hover-content">
                            <i class="fas fa-plus fa-3x"></i>
                        </div>
                    </div>
                    <img class="img-fluid" :src="require('@/assets/img/portfolio/01-full.jpg')" alt="">
                </a>
                <div class="portfolio-caption">
                    <h4>{{ obj.caption }}</h4>
                    <p class="text-muted">{{ obj.title }}</p>
                </div>
            </div>
        </div>
        </div>
    </section>
</template>

<script>

export default {
    data: () => ({
        portfolioJSON: [
            {
                img: '../assets/img/portfolio/01-full.jpg',
                caption: 'Threads',
                title: 'Illustration'
            },
            {
                img: '../assets/img/portfolio/02-full.jpg',
                caption: 'Explore',
                title: 'Graphic Design'
            },
            {
                img: '../assets/img/portfolio/03-full.jpg',
                caption: 'Finish',
                title: 'Identify'
            },
            {
                img: '../assets/img/portfolio/04-full.jpg',
                caption: 'Lines',
                title: 'Branding'
            },
            {
                img: '../assets/img/portfolio/05-full.jpg',
                caption: 'Southwest',
                title: 'Website Design'
            },
            {
                img: '../assets/img/portfolio/06-full.jpg',
                caption: 'Window',
                title: 'Photography'
            }
        ]
    })
}
</script>

<style lang="css">
</style>