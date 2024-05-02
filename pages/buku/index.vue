<template>
  <div class="content">
    <div class="container-fluid">
      <div class="row">
        <div class="col-lg-12">
          <nuxt-link to="/pengunjung">
          <button type="button" class="btn btn-outline-dark mt-4 btn-lg">KEMBALI</button></nuxt-link>
          <h2 class="text-center my-4">RAK BUKU</h2>
          <input type="search" class="form-control form-control-lg rounded-5" placeholder="Cari...">
        <div class="my-3">menampilkan 4 dari 4</div>
        <div class="row">
          <div class="col-lg-2">
            <div class="card mb-3">
              <nuxt-link to="/rincian/buku1">
                <div class="card-body">
                  <img src="@/assets/img/cover1.png" class="cover" alt="cover 1">
                </div>
              </nuxt-link>
              </div>
            </div>
            <div class="col-lg-2">
            <div class="card mb-3">
              <nuxt-link to="/rincian/buku2">
                <div class="card-body">
                  <img src="@/assets/img/cover2.png" class="cover" alt="cover 2">
                </div>
              </nuxt-link>
              </div>
            </div>
            <div class="col-lg-2">
            <div class="card mb-3">
              <nuxt-link to="/rincian/buku3">
                <div class="card-body">
                  <img src="@/assets/img/cover3.png" class="cover" alt="cover 3">
                </div>
              </nuxt-link>
            </div>
            </div>
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
.card-body {
  width: 100%;
  height: 20em;
  padding: 0;
}
.cover {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: 0 30;
}

</style>