<script setup></script>

<template>
  <div class="referance-section">
    <h1>Referanslarımız</h1>
    <div class="referance-logos">
      <a href="https://www.unkarinsaat.com.tr/index.html" target="_blank">
        <img class="unkar" src="https://www.unkarinsaat.com.tr/images/logo.png" alt="unkar-insaat">
      </a>

      <a href="https://hecahafriyat.com/ankara-kiralik-ekskavator/" target="_blank">
        <img src="https://hecahafriyat.com/wp-content/uploads/2019/06/heca-3-300x84.png" style="width: 175px;"
          alt="heca-hafriyat">
      </a>
    </div>
  </div>
</template>

<style scoped>
.referance-section {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin: 25px 0;
}
.referance-logos {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}
.referance-logos img {
  margin: 10px 30px;
  width: 250px;
}
@media (max-width: 480px) {
  .referance-logos {
    width: 100%;
  }
  .referance-logos img {
    width: 50%;
  }
  .unkar {
    transform: scale(2);
    padding-left: 20px;
  }
}
</style>