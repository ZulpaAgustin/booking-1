<template>
  <div class="container-fluid" style="background-color: #8a4848;">
    <div class="row justify-content-center tinggi p-5">
      <div class="col-5 bg-white tumpul p-3">
        <div class="icon">
        <nuxt-link class="back-button" to="http://localhost:3000/bookings"><i class="fas fa-arrow-left"></i> Kembali</nuxt-link>
      </div>
      <h2>Booking Ruang Aula</h2>
      <form id="bookingForm">
        <div class="input-group">
              <i class="fas fa-calendar-alt"></i>
              <input type="date" class="tanggal" id="tanggal" name="tanggal" placeholder="Tanggal" required>
          </div>
          <div class="input-group">
            <i class="fas fa-user"></i>
              <input type="text" class="user" name="user" placeholder="Nama Peminjam">
          </div>
          <div class="input-group">
              <i class="fas fa-calendar-check"></i>
              <input type="text" id="acara" name="acara" placeholder="Jenis Acara" required>
          </div>
          <div class="input-group time-group">
              <div class="time-input">
                  <i class="fas fa-clock"></i>
                  <input type="time" id="jamMulai" name="jamMulai" required>
              </div>
              <div class="time-input">
                  <i class="fas fa-clock"></i>
                  <input type="time" id="jamSelesai" name="jamSelesai" required>
              </div>
          </div>
          <div class="input-group">
            <div class="dropdown">
              <button class="btn btn-secondary dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">
                Pilih Alat
                <i class="fas fa-tools"></i>
              </button>
              <ul class="dropdown-menu">
                <li> <input type="checkbox" value="Sound System" class="dropdown-item"> Sound System</li>
                <li> <input type="checkbox" value="Proyektor" class="dropdown-item"> Proyektor</li>
                <li><input type="checkbox" value="Mikrofon" class="dropdown-item"> Mikrofon</li>
                <li><input type="checkbox" value="Panggung" class="dropdown-item"> Panggung</li>
              </ul>
            </div>
          </div>
          <div class="input-group jumlah-tamu">
              <i class="fas fa-users"></i>
              <input type="number" name="jumlahTamu" placeholder="Jumlah Tamu" max="150" required>
          </div>
          <div class="input-group">
              <i class="fas fa-money-bill-wave"></i>
              <input type="text" id="totalHarga" name="totalHarga" placeholder="Total Harga" readonly>
          </div>
          <button class="submit" type="submit">Booking</button>
      </form>
      <p id="message"></p>
      </div>
      
    </div>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Lexend+Deca:wght@100..900&family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&family=Rubik:ital,wght@0,300..900;1,300..900&display=swap');


h2 {
  text-align: center;
  color: #333333;
}
.tinggi{
  min-height: 100vh;
}
.tumpul{
  border-radius: 5%;
}
.input-group {
  position: relative;
  margin-bottom: 15px;
}

.input-group i {
  position: absolute;
  top: 10px;
  left: 10px;
  color: #666666;
}

.input-group.jumlah-tamu {
  margin-top: 15px;
}

.input-group input, .input-group select {
  width: 100%;
  padding: 8px 8px 8px 30px;
  box-sizing: border-box;
  border: 1px solid #cccccc;
  border-radius: 20px;
}

.time-group {
  display: flex;
  justify-content: space-between;
}

.time-input {
  position: relative;
  width: 48%;
}

.dropdown-menu {
    min-width: 455px;
    text-align: left;
}

.dropdown-item {
  display: flex;
  align-items: center;
  padding: 8px 12px;
  color: #999999;
  background-color: transparent;
}

.dropdown-item input[type="checkbox"] {
    margin-right: 10px; /* Ruang antara checkbox dan teks */
}

.dropdown-toggle {
  color: #000000;
  background-color: #fff;
  padding: 10px 187px;
  border-radius: 20px;
}

.dropdown-item:hover {
    background-color: #e9ecef; /* Warna latar belakang saat hover */
    color: #495057; /* Warna teks saat hover */
}

input::placeholder, select::placeholder {
  color: #999999;
}

.submit {
  width: 100%;
  padding: 10px;
  background-color: #601717;
  color: white;
  border: none;
  border-radius: 20px;
  cursor: pointer;
  font-size: 16px;
}

.submit:hover {
  background-color: #540b0b;
}

.back-button {
  display: inline-block;
  margin-bottom: 20px;
  text-decoration: none;
  color: #a20a0a;
  font-size: 18px;
  font-weight: bold;
}

.back-button i {
  margin-right: 8px;
}

.icon {
  margin-right: 160px;
}
</style>

<script setup>
definePageMeta({
  layout: 'layoutBooking'
})
</script>