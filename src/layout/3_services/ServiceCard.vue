<template>
    <div class="service-card service-card" :id="index">
        <card-glider :cardContent="serviceCardContent" :index="index"></card-glider>
    </div>
</template>
  
<script>
    import CardGlider from "../../components/gliders/CardGlider.vue"

    export default {
        name: "ServiceCard",
        props: {
            serviceCardContent: {
                type: Object,
                required: true
            },
            index: {
                type: Number,
                required: true
            }
        },
        components: {
            CardGlider
        }
    };
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>

  </style>
  