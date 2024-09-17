<template>
    <div class="row">
      <div class="col">
      <section class="home">
          <div class="content">
            <Carousel />
          </div>
        </section>
      </div>
    </div>
    <br>
        <section class="ruang">
          <div class="container top">
            <div class="heading">
              <h1>TERSEDIA</h1>
              <h2>Paket Aula</h2>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sit repellat quia, doloribus necessitatibus rem soluta distinctio cum quam neque? Necessitatibus officiis error nobis voluptatum magni, consectetur quibusdam corrupti officia iusto.</p>
            </div>
          </div>
          <!-- Carousel -->
   
    <!-- Baris Paket -->
  <div id="packageCarousel" class="carousel slide" data-bs-ride="carousel">
    <div class="carousel-inner">
      <div class="carousel-item active">
        <div class="row">
          <div class="col-md-4">
            <div class="card">
              <img src="/assets/img/ruang.jpg" class="card-img-top" alt="Paket A">
              <div class="card-body">
                <h5 class="card-title">Paket A</h5>
                <p class="card-text">
                  <i class="fa-solid fa-user-group"></i> Untuk 25 orang <br>
                  <i class="fas fa-tools"></i> 2 mikrofon dan 1 sound system.
                </p>
                <NuxtLink to="#" class="btn btn-dark"> Check-In</NuxtLink>
              </div>
            </div>
          </div>
          <div class="col-md-4">
            <div class="card">
              <img src="/assets/img/ruang.jpg" class="card-img-top" alt="Paket B">
              <div class="card-body">
                <h5 class="card-title">Paket B</h5>
                <p class="card-text">
                  <i class="fa-solid fa-user-group"></i> Untuk 50 orang <br>
                  <i class="fas fa-tools"></i> 4 mikrofon dan 2 sound system.
                </p>
                <NuxtLink to="#" class="btn btn-dark"> Check-In</NuxtLink>
              </div>
            </div>
          </div>
          <div class="col-md-4">
            <div class="card">
              <img src="/assets/img/ruang.jpg" class="card-img-top" alt="Paket C">
              <div class="card-body">
                <h5 class="card-title">Paket C</h5>
                <p class="card-text">
                  <i class="fa-solid fa-user-group"></i> Untuk 100 orang <br>
                  <i class="fas fa-tools"></i> 6 mikrofon dan 4 sound system.
                </p>
                <NuxtLink to="#" class="btn btn-dark"> Check-In</NuxtLink>
              </div>
            </div>
          </div>
        </div>
        </div>
        
         <!-- Paket D (paket baru) -->
      <div class="carousel-item">
        <div class="row">
          <!-- Paket D -->
          <div class="col-md-4">
            <div class="card">
              <img src="/assets/img/ruang.jpg" class="card-img-top" alt="Paket D">
              <div class="card-body">
                <h5 class="card-title">Paket D</h5>
                <p class="card-text"><i class="fa-solid fa-user-group"></i> Untuk 150 orang <br>
                   <i class="fas fa-tools"></i> 8 mikrofon dan 6 sound system.</p>
                   <NuxtLink to="#" class="btn btn-dark"> Check-In</NuxtLink>
              </div>
            </div>
          </div>
          <!-- Paket E -->
          <div class="col-md-4">
            <div class="card">
              <img src="/assets/img/ruang.jpg" class="card-img-top" alt="Paket D">
              <div class="card-body">
                <h5 class="card-title">Paket E</h5>
                <p class="card-text"><i class="fa-solid fa-user-group"></i> Untuk 200 orang <br>
                  <i class="fas fa-tools"></i> 10 mikrofon dan 8 sound system.</p>
                  <NuxtLink to="#" class="btn btn-dark"> Check-In</NuxtLink>
              </div>
            </div>
          </div>
          <!-- Paket F -->
          <div class="col-md-4">
            <div class="card">
              <img src="/assets/img/ruang.jpg" class="card-img-top" alt="Paket D">
              <div class="card-body">
                <h5 class="card-title">Paket F</h5>
                <p class="card-text"><i class="fa-solid fa-user-group"></i> Untuk 250 orang <br>
                  <i class="fas fa-tools"></i> 12 mikrofon dan 10 sound system.</p>
                  <NuxtLink to="#" class="btn btn-dark"> Check-In</NuxtLink>
              </div>
            </div>
          </div>
          <!--  -->
        </div>
      </div>
      </div>
    
  
    <!-- Kontrol panah -->
    <a class="carousel-control-prev" href="#packageCarousel" role="button" data-bs-slide="prev">
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Sebelumnya</span>
    </a>
    <a class="carousel-control-next" href="#packageCarousel" role="button" data-bs-slide="next">
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Berikutnya</span>
    </a>
  </div>
        </section>
  
   
  <div class="footer">
    <footer>The Pranksters</footer>
  </div>
  
  </template>
  
  <style>
  @import url('https://fonts.googleapis.com/css2?family=Lexend+Deca:wght@100..900&family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&family=Rubik:ital,wght@0,300..900;1,300..900&display=swap');
  
  * {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }
  
  body {
    font-family: 'Poppins', sans-serif;
  }
  
  h1, h2 {
    font-family: sans-serif;
    font-weight: 400px;
  }
  
  a {
    text-decoration: none;
  }
  
  li {
    list-style: none;
  }
  
  .flex {
    display: flex;
  }
  
  .flex_space {
    display: flex;
    justify-content: space-between;
  }
  
  .container {
    max-width: 85%;
    margin: auto;
  }
  .home {
    height: 100vh;
    color: #fff;
  }
  
  button {
    border: none;
    background: none;
    outline: none;
    transition: 0.5s;
    cursor: pointer;
  }
  
  .primary-btn {
    padding: 15px 40px;
    background: #7e2d2d;
    font-weight: bold;
    color: white;
  }
  
  .home img {
    width: 100%;
    min-height: 100px;
    background-repeat: no-repeat;
  }
  
  .home .text {
    position: absolute;
    top: 35%;
    left: 5%;
  }
  
  .home .text h1 {
    font-size: 80px;
    font-family: serif;
    font-weight: 400;
  }
  
  .home p{
    margin: 20px 0;
    font-size: 20px;
    font-family:'Times New Roman', Times, serif
  }
  
  .home button {
    margin-right: 20px;
  }
  
  .carousel-control-prev {
    top: 45%;
    height: 50px;
    width: 50px;
    background: #0000005e;
    color: #fff;
    border-radius: 10px;
  }
  .carousel-control-next {
    top: 45%;
    height: 50px;
    width: 50px;
    background: #0000005e;
    color: #fff;
    border-radius: 10px;
  }
  
  .top {
    margin-top: 80px;
  }
  
  .mtop {
    margin-top: 40px;
  }
  
.heading {
  margin-left: 0px;
}

  .heading h1 {
    font-size: 100px;
    font-weight: 500;
    opacity: 0.1;
    font-family: serif;
    position: absolute;
    top: -30px;
  }
  
  .heading h2 {
    margin: 30px 0;
    font-size: 45px;
    font-family: serif;
    font-weight: 400;
  }
  
  .container {
    justify-content: center;
    align-items: center;
  }
  
  .ruang {
    position: relative;
  }
  
  footer{
    background-color: rgb(151, 64, 42);
    position: sticky;
    bottom: 0px;
    display: flex;
    justify-content: center;
  }
  </style>
  
  <script setup>
  useHead({
    title: "Home"
  })
  
  
  </script>
  
  <!-- <template>
    <div>Halo</div>
  </template> -->