<template>
  <div class="container-fluid">
    <div class="content">
      <div class="row">
        <div class="col-lg-12 ">
          <form>
            <h2 class="text-center my-4 text-light">ISI DATA KUNJUNGAN</h2>
            <div class="mb-3">
              <input type="text" class="form-control form-control-lg rounded-5" placeholder="Nama ...">
            </div>

            <div class="mb-3">
              <select v-model="keanggotaan" class="form-control form-control-lg form-select rounded-5">
                <option value="">KEANGGOTAAN</option>
                <option value="Siswa">Siswa</option>
                <option value="Guru">Guru</option>
                <option value="Staf">Staf</option>
                <option value="Umum">Umum</option>
              </select>
              </div>

            <div class="mb-3" v-if="keanggotaan == 'Siswa'">
              <div class="row">
                <div class="col-md-4">
                  <select class="form-control form-control-lg form-select rounded-5 mb-2">
                    <option value="">TINGKAT</option>
                    <option value="X">X</option>
                    <option value="XI">XI</option>
                    <option value="XII">XII</option>
                </select>
                </div>

                <div class="col-md-4">
                <select class="form-control form-control-lg form-select rounded-5 mb-2">
                  <option value="">JURUSAN</option>
                  <option value="PPLG">PPLG</option>
                  <option value="TJKT">TJKT</option>
                  <option value="TSM">TSM</option>
                  <option value="DKV">DKV</option>
                  <option value="TOI">TOI</option>
                  </select>
                </div>

                <div class="col-md-4">
                  <select class="form-control form-control-lg form-select rounded-5 mb-2">
                  <option value="">KELAS</option>
                  <option value="1">1</option>
                  <option value="2">2</option>
                  <option value="3">3</option>
                  <option value="4">4</option>
                  </select>
                </div>
              </div>
            </div>

            <div class="mb-3">
              <select  class="form-control form-control-lg form-select rounded-5">
                <option value="">KEPERLUAN</option>
                <option value="baca">Baca Buku</option>
                <option value="pinjam">Pinjam Buku</option>
                <option value="kembalikan">kembalikan Buku</option>
              </select>
            </div>
            <nuxt-link to="/pengunjung">
            <button type="submit" class="btn btn-dark btn-lg rounded-5 px-5">SUBMIT</button>
            </nuxt-link>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>

const keanggotaan = ref('')
</script>

<style scoped>
.content {
  width: 100%;
  height: 500px;
  padding-top: 150px;
  display: flex;
  justify-content: space-evenly;
  flex-direction: row;
  flex-wrap: wrap;
  align-content: center;
}
form {
  background-image:linear-gradient(#808080,#ffffff)  ;
  padding: 1rem;
  border-radius: 20px;
}
.container-fluid {
  background-image: url("@/assets/img/bg.png");
  background-size:cover;
  width: 100%;
  height: 100vh;
}
</style>