<template>
  <div class="badan">
  <div class="container">
    <div class="row">
        <div class="col-lg-12">
          <div class="icon">
            <nuxt-link class="back-button" to="http://localhost:3000/bookings"><i class="fas fa-arrow-left"></i> Kembali</nuxt-link>
          </div>
            <h2 class="text">Rekapan Data</h2>
            <div class="table-controls">
                <div class="ms-auto">
                    <div class="search-container">
                        <i class="fa fa-search search-icon"></i>
                        <input type="text" id="searchInput" placeholder="Cari Nama...">
                    </div>
                  </div>
                </div>
            </div>
        </div>
    <div class="my-3 text-white">Menampilkan {} Dari {} Peminjam</div>
    <table>
        <thead>
            <tr class="bgrcolor">
                <th>No</th>
                <th>Pemesan</th>
                <th>Tanggal Booking</th>                    
                <th>Jam Mulai</th>
                <th>Jam Selesai</th>
                <th>Total Bayar</th>
            </tr>
        </thead>
        <tbody>
            <tr class="bgcolor">
              <th>1</th>
              <th>Lisye Diana</th>
              <th>20-02-2024</th>
              <th>11.00</th>
              <th>12.00</th>
              <th>100.000</th>
            </tr>
        </tbody>
    </table>

    <div class="total-bayar text-white">
        <p>Total Keseluruhan : {}</p>
    </div>
</div>
</div>

</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Lexend+Deca:wght@100..900&family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&family=Rubik:ital,wght@0,300..900;1,300..900&display=swap');

* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

.badan {
  margin: 0;
  padding: 0;
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

.icon {
  margin-right: 160px;
}

.back-button {
    display: inline-block;
    margin-bottom: 20px;
    text-decoration: none;
    color: #ffffff;
    font-size: 18px;
    font-weight: bold;
}

.container {
  background-color: #a03636;
  padding: 2em;
  max-width: 100%;
}

table {
  width: 100%;
  border-collapse: collapse;
  margin: 2em 0;
}

table, th, td {
  border: 1px solid #000000;
}

th, td {
  padding: 1em;
  text-align: left;
}

.bgrcolor {
  background-color: #e07171;
}

.bgcolor {
  background-color: rgb(255, 255, 255)
}

.status-ongoing {
  color: red;
}

.status-ended {
  color: rgb(109, 104, 104);
}

.table-controls {
  display: flex;
  justify-content: space-between;
  margin-bottom: 15px;
}

#searchInput {
  padding: 5px 5px 5px 30px; /* Tambahkan padding kiri untuk memberi ruang pada ikon */
  border: 1px solid #ccc;
  border-radius: 4px;
}

.search-container {
  position: relative;
  display: inline-block;
}

.search-icon {
  position: absolute;
  left: 10px;
  top: 50%;
  transform: translateY(-50%);
  color: #000000;
}

.text {
  text-align: center;
  color: #fff;
}
</style>