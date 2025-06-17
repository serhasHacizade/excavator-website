<script setup>

</script>

<template>
    <div class="service-section" id="service-section">
        <p class="service-section-p"> <span class="service-section-span">Hitachi 250LCH</span> 25 tonluk ekskavatörümüz,
            saatlik, günlük, haftalık ve yıllık olmak
            üzere operatörlü veya operatörsüz olarak kiralanabilmektedir. Türkiye’nin tüm şehirlerine hizmet veriyoruz.
            Güçlü makine parkurumuz ve profesyonel ekibimizle, projelerinize zamanında ve güvenilir çözümler sunuyoruz.
        </p>
        <div class="services">
            <a-card class="service-section-card" hoverable>
                <template #cover>
                    <img alt="example" src="/temel-kazim.jpg" />
                </template>
                <a-card-meta class="service-section-meta" title="TEMEL KAZIM">
                    <template #description>Sağlam yapıların ilk adımı için güvenilir ve hassas kazı hizmeti
                        sunuyoruz.</template>
                </a-card-meta>
            </a-card>

            <a-card class="service-section-card" hoverable>
                <template #cover>
                    <img alt="example" src="/moloz-temizligi.jpg" />
                </template>
                <a-card-meta class="service-section-meta" title="MOLOZ TEMİZLİĞİ">
                    <template #description>Şantiye ve inşaat alanlarınızda hızlı ve düzenli moloz tahliyesi
                        sağlıyoruz.</template>
                </a-card-meta>
            </a-card>

            <a-card class="service-section-card" hoverable>
                <template #cover>
                    <img alt="example" src="/tesviye.jpg" />
                </template>
                <a-card-meta class="service-section-meta" title="TESVİYE">
                    <template #description>İnşaat öncesi ve sonrası zeminleri profesyonelce düzeltiyoruz.</template>
                </a-card-meta>
            </a-card>
        </div>
    </div>
</template>

<style scoped>
.service-section {
    width: 100%;
}

.service-section-p {
    line-height: 2.4rem;
    font-size: 20px;
    color: rgb(107, 107, 107);
    width: 80%;
    margin: 10px auto;
    text-align: center;
}

.service-section-span {
    font-weight: bold;
    color: black;
}

.services {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: 35px auto;
    width: 80%;
}

.service-section-card {
    margin: 5px 40px;
    height: 410px;
}

.service-section-meta {
    font-size: 20px;
}

@media (max-width: 480px) {
    .service-section {
        min-width: 100%;
    }

    .services {
        min-width: 30%;
        flex-wrap: wrap;
    }
    
    .service-section-card {
        min-width: 10%;
        margin: 55px auto;
        width: 320px !important;
        height: 300px;
    }

    .service-section-meta {
        font-size: 20px;
        width: 80%;
    }

    .service-section-meta :deep(.ant-card-meta-title) {
        font-size: 22px;
        font-weight: bold;
    }
    .service-section-p {
        font-size: 30px;
        line-height: 2.5rem;
    }
}

@media (max-width: 768px) {
    .service-section {
        width: 100%;
    }
    
    .service-section-p {
        width: 90%;
        margin: 0 auto;
        font-size: 20px;
        line-height: 1.8rem;
    }
    .services {
        margin: 150px auto;
        width: 85%;
        flex-direction: column;
    }

    .service-section-card {
        width: 420px;
        height: 450px;
    }

}

@media (max-width: 1024px) {
    .services {
        width: 95%;
    }
    .service-section-p {
        min-width: 70%;
    }
}

@media (max-width: 1280px) {
    .service-section {
        width: 100%;
    }
}
</style>