<script setup>
import Navbar from './components/Navbar.vue';
import Info from './components/Info.vue';
import Service from './components/Service.vue';
import Carousel from './components/Carousel.vue';
import Referance from './components/Referance.vue';
import About from './components/About.vue';

import { ref, onMounted } from 'vue';
import { Spin } from 'ant-design-vue';

const loading = ref(true);

onMounted(() => {
  setTimeout(() => {
    loading.value = false;
  }, 1500);
});
</script>

<template>
  <div>

    <div>
      <a-spin size="large" tip="Yükleniyor..." v-if="loading" class="loader" />

      <transition name="fade">
        <div v-show="!loading">
          <!-- Asıl site içeriğin burada -->
          <Navbar />
          <!-- diğer tüm içeriğin (carousel, service-section vs) -->
          <Info />
          <Service />
          <Carousel />
          <Referance />
          <About />
        </div>
      </transition>
    </div>
  </div>
</template>

<style scoped>
.loader {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

/* Fade geçişi */
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.8s;
}

.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}
</style>
