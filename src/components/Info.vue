<script setup></script>

<template>
    <div class="info-section" id="info-section">
        <img src="/excavator-img.png" alt="excavator-img" class="info-section-img">
        <div class="title-info">
            <h1 class="info-section-h1">GÜVENİLİR <br> KAZI VE HAFRİYAT HİZMETLERİ</h1>
            <p class="info-section-p">25 tonluk profesyonel kepçemiz ile <br> temel kazım, moloz temizliği, <br> tesviye
                ve
                daha fazlası</p>
        </div>
    </div>
</template>

<style scoped>
.info-section {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 110px 0 70px 0;
}
.title-info {
    width: 30%;
}
.info-section-h1 {
    line-height: 2.5rem;
}
.info-section-p {
    line-height: 1.4rem;
    font-weight: 700;
    color: rgb(107, 107, 107);
}



@media (max-width: 480px) {
    .info-section {
        flex-direction: column;
        width: 100%;
        padding-top: 175px;
    }

    .title-info {
        text-align: center;
    }

    .info-section-h1 {
        line-height: 2.5rem;
    }
    
    .info-section-p {
        font-size: x-large;
    }
}
@media (max-width: 768px) {
    .info-section {
        margin: 0 auto;
        flex-direction: column;
    }
    .info-section-img {
        max-width: 95%;
        margin: 0;
    }
    .title-info {
        width: 90%;
        font-size: medium;
        text-align: center;
    }
    .info-section-p {
        font-size: 20px;
        text-align: center;
        
    }
}
@media (max-width: 1024px) {
    .info-section-h1 {
        min-width: 250px;
        
    }
    .info-section-p {
        min-width: 250px;
    }
}
</style>