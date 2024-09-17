<template>
  <div class="container-fluid">
    <section>
      <Panel />
    </section>
    <div class="main-content">
      <h1 class="text text-center">Daftar Peminjam</h1>
      <table class="table mt-3 mt-4">
            <thead class="table-dark">
              <tr>
                <td>No</td>
                <td>Pemesan</td>
                <td>Tanggal</td>
                <td>Jam Mulai</td>
                <td>Jam Selesai</td>
                <td>Bayar</td>
                <td>Terima</td>
                <td>Tolak</td>
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
                <td><i class="bi bi-check-square-fill"></i></td>
                <td><i class="bi bi-x-square-fill"></i></td>
              </tr>
            </tbody>
          </table>
          <p>Total Semua : {}</p>
    </div>
  </div>
</template>

<script setup>
definePageMeta({
  layout: 'layoutBooking'
})
</script>

<style scoped>

</style>