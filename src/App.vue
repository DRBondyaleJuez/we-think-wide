<script setup>
import HeaderView from './layout/1_header/HeaderView.vue'

import MediaInteractiveDisplay from './layout/2_media_interactive_display/MediaInteractiveDisplay.vue'
import Services from './layout/3_services/Services.vue'
import SpecializedServices from './layout/4_specialized_services/SpecializedServices.vue'
import Projects from './layout/5_projects/Projects.vue'
import Interihotel from './layout/6_interihotel/Interihotel.vue'
import Ecosystem from './layout/7_ecosystem/Ecosystem.vue'
import Clients from './layout/8_clients/Clients.vue'
import FooterView from './layout/9_footer/FooterView.vue'


import introduction from './assets/static/json/introduction.json';

</script>

<template>
  <main>
    <HeaderView />
    <MediaInteractiveDisplay />
    <div class="content-wrapper">
      <h3 class="introduction">
        {{ introduction.text }}
      </h3>
      <Services />
      <SpecializedServices />
      <Projects />
      <Interihotel />
      <!--<Ecosystem />
      <Clients />-->
    </div>
    <FooterView />
  </main>

</template>

<style scoped>
/*header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}*/
</style>
