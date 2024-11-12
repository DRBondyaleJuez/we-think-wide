<template>
    <div class="glide">
        <div class="glide__track" data-glide-el="track">
          <ul class="glide__slides">
            <li class="glide__slide">0</li>
            <li class="glide__slide">1</li>
            <li class="glide__slide">2</li>
          </ul>
        </div>
        <div class="glide__arrows" data-glide-el="controls">
            <button class="glide__arrow glide__arrow--left" data-glide-dir="<">prev</button>
            <button class="glide__arrow glide__arrow--right" data-glide-dir=">">next</button>
          </div>
      </div>      
</template>

<script>
 import Glide from '@glidejs/glide';

export default {
    name: "TestGlider",
    props: {
    },
    data() { 
        return {
        };
    },
    mounted() {
        this.setGlider();
    }, 
    methods: {
        setGlider() {
            const config = {
                type: 'carousel',
                startAt: 0,
                perView: 1,
                autoplay: 2000,
                gap: 0

            }
            let currentGlide = new Glide('.glide', config).mount({})
            
        },
    }   
};
</script>