<script setup>
import { LeftCircleOutlined, RightCircleOutlined } from '@ant-design/icons-vue';

</script>

<template>
    <div class="carousel-section" id="carousel-section">
        <a-carousel arrows>
            <template #prevArrow>
                <div class="custom-slick-arrow left">
                    <left-circle-outlined />
                </div>
            </template>
            <template #nextArrow>
                <div class="custom-slick-arrow right">
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
    width: 100%;
}

.carousel-image-container {
    height: 100%;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 0 12px;
    box-sizing: border-box;
}

.carousel-image-container img {
    width: 100%;
    max-width: 600px;
    height: auto;
    object-fit: cover;
}

.custom-slick-arrow.left {
    position: absolute;
    left: 300px;
    z-index: 1;
}

.custom-slick-arrow.right {
    position: absolute;
    right: 300px;
    z-index: 5;
}

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

@media (max-width: 480px) {
    .carousel-image-container {
        padding: 0;
    }

    .carousel-image-container img {
        max-width: 100%;
        height: auto;
    }

    .custom-slick-arrow.left {
        left: 15px;
    }

    .custom-slick-arrow.right {
        right: 15px;
    }
}

@media (max-width: 768px) {
    .custom-slick-arrow.left {
        left: 30px;
    }

    .custom-slick-arrow.right {
        right: 30px;
    }
}

@media (max-width: 1024px) {
    .custom-slick-arrow.left {
        left: 50px;
    }

    .custom-slick-arrow.right {
        right: 50px;
    }
}
</style>