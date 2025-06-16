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

            <a-card class="service-section-card" hoverable style="width: 240px">
                <template #cover>
                    <img alt="example" src="/temel-kazim.jpg" />
                </template>
                <a-card-meta title="TEMEL KAZIM">
                    <template #description>Sağlam yapıların ilk adımı için güvenilir ve hassas kazı hizmeti
                        sunuyoruz.</template>
                </a-card-meta>
            </a-card>

            <a-card class="service-section-card" hoverable style="width: 240px">
                <template #cover>
                    <img alt="example" src="/moloz-temizligi.jpg" />
                </template>
                <a-card-meta title="MOLOZ TEMİZLİĞİ">
                    <template #description>Şantiye ve inşaat alanlarınızda hızlı ve düzenli moloz tahliyesi
                        sağlıyoruz.</template>
                </a-card-meta>
            </a-card>

            <a-card class="service-section-card" hoverable style="width: 240px">
                <template #cover>
                    <img alt="example" src="/tesviye.jpg" />
                </template>
                <a-card-meta title="TESVİYE">
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
    line-height: 1.4rem;
    color: rgb(107, 107, 107);
    width: 60%;
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
    width: 60%;
}

.service-section-card {
    margin: 5px 50px;
}
</style>