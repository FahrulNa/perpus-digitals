<template>
  <div class="content">
    <nuxt-link to="../" class="ms-3">
          <button type="button" class="btn btn-outline-dark btn-lg">ISI DATA</button></nuxt-link>
    <div class="container-fluid d-flex justify-content-center">
      <div class="row">
        <div class="row-lg py-5">
          <div class="col">
            <nuxt-link to="/pengunjung/tambah" class="text-decoration-none">
            <div class="card bg-pengunjung rounded-5">
              <div class="card-body pt-5">
                <h2 class="mt-5">RIWAYAT KUNJUNGAN</h2>
              </div>
            </div>
          </nuxt-link>
          </div>
        </div>
        <div class="row-lg">
          <div class="col">
            <nuxt-link to="/buku" class="text-decoration-none">
              <div class="card bg-buku rounded-5">
                <div class="card-body pt-5">
                  <h2 class="mt-5">CARI BUKU</h2>
                </div>
              </div>
            </nuxt-link>
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
.card {
  opacity: 80%;
  color: white;
  align-items: center;
  height:250px;
  box-shadow: 1px 1px 10px #424242;
}
.card.bg-pengunjung {
  background-image: url('@/assets/img/bgvisit.png');
  background-repeat: no-repeat;
  background-position: center center;
  background-size: cover;
}
.card.bg-buku {
  background: url('@/assets/img/bgsearch.png');
  background-size: cover;
}
</style>
