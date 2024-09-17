<template>
  <div class="container-fluid">
    <section>
      <Panel />
    </section>
    <!-- Main Content -->
<div class="main-content">
  <h1 class="text text-center">Selamat Datang di Halaman Admin</h1>

  <!-- Card Section -->
  <div class="row">
    <!-- Card 1: Peminjam -->
    <div class="col-md-6">
      <div class="card text-center mb-4">
        <div class="card-body">
          <i class="bi bi-person-badge-fill"></i>
          <h5 class="card-title">Peminjam</h5>
          <p class="card-text">Informasi tentang peminjam aula</p>
        </div>
      </div>
    </div>
    <!-- Card 2: Admin -->
    <div class="col-md-6">
      <div class="card text-center mb-4">
        <div class="card-body">
          <i class="bi bi-people-fill"></i>
          <h5 class="card-title">Admin</h5>
          <p class="card-text">Informasi tentang admin</p>
        </div>
      </div>
    </div>
  </div>
  <div class="bag-table">
    <h4 class="text text-center mt-3">Riwayat Peminjam</h4>
  <table class="table mt-3">
            <thead class="table-dark">
              <tr>
                <td>No</td>
                <td>Pemesan</td>
                <td>Tanggal</td>
                <td>Jam Mulai</td>
                <td>Jam Selesai</td>
                <td>Bayar</td>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>1</td>
                <td>Lisye Diana</td>
                <td>2024-07-12</td>
                <td>10.00</td>
                <td>11.00</td>
                <td>100.000</td>
              </tr>
              <tr>
                <td>2</td>
                <td>Lisye Diana</td>
                <td>2024-08-13</td>
                <td>10.00</td>
                <td>11.00</td>
                <td>100.000</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
  </div>
</template>

<script setup>
definePageMeta({
  layout: 'layoutBooking'
})
</script>