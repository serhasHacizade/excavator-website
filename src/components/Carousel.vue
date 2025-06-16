<script setup>
import { LeftCircleOutlined, RightCircleOutlined } from '@ant-design/icons-vue';

</script>

<template>
    <div class="carousel-section" id="carousel-section">
        <a-carousel arrows>
            <template #prevArrow>
                <div class="custom-slick-arrow" style="left: 200px; z-index: 1">
                    <left-circle-outlined />
                </div>
            </template>
            <template #nextArrow>
                <div class="custom-slick-arrow" style="right: 200px">
                    <right-circle-outlined />
                </div>
            </template>
            <div class="carousel-image-container">
                <img src="/img-1.jpg" alt="">
            </div>
            <div class="carousel-image-container">
                <img src="/img-2.jpg" alt="">
            </div>
            <div class="carousel-image-container">
                <img src="/img-3.jpg" alt="">
            </div>
            <div class="carousel-image-container">
                <img src="/img-4.jpg" alt="">
            </div>
            <div class="carousel-image-container">
                <img src="/img-5.jpg" alt="">
            </div>
            <div class="carousel-image-container">
                <img src="/img-6.jpg" alt="">
            </div>
        </a-carousel>
    </div>
</template>

<style scoped>
.carousel-section {
    height: 450px;
    background-color: #2f487a;
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;
    margin: 55px auto;
}

:deep(.ant-carousel) {
    height: 100%;
    width: 100%;
}

.carousel-image-container {
    height: 100%;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
}

.carousel-image-container img {
    height: 60%;
    width: 600px;
    object-fit: cover;
}

/* For demo */
:deep(.slick-slide) {
  height: 100%;
  display: flex !important;
  justify-content: center;
  align-items: center;
}

:deep(.slick-arrow.custom-slick-arrow) {
  width: 25px;
  height: 25px;
  font-size: 25px;
  color: #fff;
  background-color: rgba(31, 45, 61, 0.11);
  transition: ease all 0.3s;
  opacity: 0.3;
  z-index: 1;
}

:deep(.slick-arrow.custom-slick-arrow:before) {
  display: none;
}

:deep(.slick-arrow.custom-slick-arrow:hover) {
  color: #fff;
  opacity: 0.5;
}

:deep(.slick-slide h3) {
  color: #fff;
}
</style>