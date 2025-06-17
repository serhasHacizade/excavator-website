<script setup>
const scrollTo = (sectionId) => {
    const section = document.getElementById(sectionId);
    section?.scrollIntoView({ behavior: 'smooth' })
};
</script>

<template>
    <div class="navbar-container">
        <img src="/logo.png" class="logo-img" alt="">
        <h2>BK KEPÇE OPERATÖRLÜĞÜ</h2>
        <div class="navbar-right-side">
            <a-space>
                <a-button class="navbar-btn" @click="scrollTo('service-section')" type="text"
                    size="large">Hizmetler</a-button>
                <a-button class="navbar-btn" @click="scrollTo('carousel-section')" type="text"
                    size="large">Çalışmalarımız</a-button>
                <a-button class="navbar-btn" @click="scrollTo('about-section')" type="text"
                    size="large">İletişim</a-button>
            </a-space>
        </div>
    </div>
</template>

<style scoped>
.navbar-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: fixed;
    background-color: white;
    width: 100%;
    z-index: 25;
    padding: 0 25px;
}

.logo-section {
    display: flex;
    justify-content: center;
    align-items: center;
}

.logo-img {
    width: 80px;
}

.navbar-right-side {
    margin-right: 35px;
}

@media (max-width: 480px) {
    .logo-img {
        width: 80px;
    }
    h2 {
        margin-right: 5%;
        font-size: 25px;
    }
}

@media (max-width: 768px) {
    .navbar-container {
        width: 92%;
    }
    .navbar-btn {
        padding-bottom: 40px;
        font-size: 20px;
        font-weight: 500;
    }
    .navbar-right-side {
        display: none;
    }
    h2 {
        font-size: 18px;
    }
}

@media (max-width: 1024px) {
    .navbar-btn {
        padding-bottom: 30px;
        font-size: 15px;
        font-weight: 400;
    }
}
</style>
