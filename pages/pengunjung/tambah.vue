<template>
  <div class="content">
    <div class="container-fluid">
      <div class="row">
        <div class="col-lg-12">
          <nuxt-link to="/pengunjung">
          <button type="button" class="btn btn-outline-dark mt-4 btn-lg">KEMBALI</button></nuxt-link>
          <h2 class="text-center my-4">RIWAYAT KUNJUNGAN</h2>
          <div class="my-3">
            <input type="search" class="form-control form-control-lg rounded-5" placeholder="Cari...">
          </div>
          <div class="my-3">menampilkan 1 dari 1</div>
          <div class="table-responsive">
            <table class="table table-bordered border-dark">
            <thead>
              <tr>
                <td>ID</td>
                <td>NAMA</td>
                <td>KEANGGOTAAN</td>
                <td>KELAS</td>
                <td>KEPERLUAN</td>
                <td>TANGGAL</td>
                <td>JAM</td>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>1.</td>
                <td>fahrul</td>
                <td>Siswa</td>
                <td>XI PPLG 3</td>
                <td>Baca</td>
                <td>22 Februari 2024</td>
                <td>10.20.00</td>
              </tr>
            </tbody>
          </table>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped>
.content{
  background-image: linear-gradient(#808080,#ffffff);
  font-family: "";
}
.h2{
  color:white;
}
</style>