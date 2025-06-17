<script setup>

</script>

<template>
    <div class="about-section" id="about-section">
        <div class="person-about">
            <img src="/BK-makine.jpg" alt="BK-makine" class="person-about-img">
            <div class="about-section-info">
                <h1 class="about-section-h1">BİZİMLE İLETİŞİME GEÇİN</h1>
                <h3>Batuhan KAPAN</h3>
                <div class="info">
                    <svg xmlns="http://www.w3.org/2000/svg" width="25" height="25" fill="currentColor"
                        class="bi bi-telephone" viewBox="0 0 16 16">
                        <path
                            d="M3.654 1.328a.678.678 0 0 0-1.015-.063L1.605 2.3c-.483.484-.661 1.169-.45 1.77a17.6 17.6 0 0 0 4.168 6.608 17.6 17.6 0 0 0 6.608 4.168c.601.211 1.286.033 1.77-.45l1.034-1.034a.678.678 0 0 0-.063-1.015l-2.307-1.794a.68.68 0 0 0-.58-.122l-2.19.547a1.75 1.75 0 0 1-1.657-.459L5.482 8.062a1.75 1.75 0 0 1-.46-1.657l.548-2.19a.68.68 0 0 0-.122-.58zM1.884.511a1.745 1.745 0 0 1 2.612.163L6.29 2.98c.329.423.445.974.315 1.494l-.547 2.19a.68.68 0 0 0 .178.643l2.457 2.457a.68.68 0 0 0 .644.178l2.189-.547a1.75 1.75 0 0 1 1.494.315l2.306 1.794c.829.645.905 1.87.163 2.611l-1.034 1.034c-.74.74-1.846 1.065-2.877.702a18.6 18.6 0 0 1-7.01-4.42 18.6 18.6 0 0 1-4.42-7.009c-.362-1.03-.037-2.137.703-2.877z" />
                    </svg>
                    <div>05400281558 05380281558</div>
                </div>

                <div class="info">
                    <svg xmlns="http://www.w3.org/2000/svg" width="25" height="25" fill="currentColor"
                        class="bi bi-mailbox-flag" viewBox="0 0 16 16">
                        <path
                            d="M10.5 8.5V3.707l.854-.853A.5.5 0 0 0 11.5 2.5v-2A.5.5 0 0 0 11 0H9.5a.5.5 0 0 0-.5.5v8zM5 7c0 .334-.164.264-.415.157C4.42 7.087 4.218 7 4 7s-.42.086-.585.157C3.164 7.264 3 7.334 3 7a1 1 0 0 1 2 0" />
                        <path
                            d="M4 3h4v1H6.646A4 4 0 0 1 8 7v6h7V7a3 3 0 0 0-3-3V3a4 4 0 0 1 4 4v6a1 1 0 0 1-1 1H1a1 1 0 0 1-1-1V7a4 4 0 0 1 4-4m0 1a3 3 0 0 0-3 3v6h6V7a3 3 0 0 0-3-3" />
                    </svg>
                    <div>bkmakinee@gmail.com</div>
                </div>

                <div class="info">
                    <svg xmlns="http://www.w3.org/2000/svg" width="25" height="25" fill="currentColor"
                        class="bi bi-caret-down" viewBox="0 0 16 16">
                        <path
                            d="M3.204 5h9.592L8 10.481zm-.753.659 4.796 5.48a1 1 0 0 0 1.506 0l4.796-5.48c.566-.647.106-1.659-.753-1.659H3.204a1 1 0 0 0-.753 1.659" />
                    </svg>
                    <div>Sivas/MERKEZ</div>
                </div>


            </div>

        </div>
    </div>
</template>

<style scoped>
.about-section {
  background-color: #2f487a;
  padding: 50px 0;
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
}

.about-section-info {
  margin-left: 55px;
  border-left: 1px solid white;
  padding-left: 25px;
  
}

.person-about {
  display: flex;
  width: 80%;
  margin: 0 auto;
 
}

.person-about-img {
  width: 450px;
  background-color: #2f487a;
}

.info {
  display: flex;
  justify-content: baseline;
  align-items: center;
  margin: 10px 0;
}

.info>* {
  font-size: 25px;
  margin-right: 10px;
}

@media (max-width: 480px) {
  .about-section {
    padding: 0;
  }
  .person-about {
    display: flex;
    flex-direction: column;
  }
  .person-about-img {
    width: 60%;
    margin: 25px 0;
  }
  .about-section-info {
    margin: 0;
    padding-bottom: 20px;
  }
}

@media (max-width: 768px) {
  .person-about-img {
    width: 50%;
    padding-left: 0;
  }
  .about-section-info {
    font-size: 7px;
    margin: 10px;
  }
  h3 {
    font-size: 17px;
  }
}
@media (max-width: 1024px) {
  .person-about-img {
    width: 40%;
  }
}


</style>