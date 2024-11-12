<template>
    <div class="services">
        <h2>Servicios</h2>
        <div class="services__cards">
            <div v-for="(servicesItem, index) in servicesList" :key="index">
                <service-card :service-card-content=servicesItem.cardContent :index="index"></service-card>
            </div>
        </div>

    </div>
</template>
  
<script>
    import ServiceCard from "./ServiceCard.vue"
    import servicesCardList from './services-card-list.json';

  export default {
    name: "Services",
    components: {
        ServiceCard
    },
    data() { 
        return {
            servicesList: servicesCardList
        };
    },
  };
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
  </style>