<template>
  <div>
    <b-navbar toggleable="lg" type="light" class="navbar fixed-top">
      <div class="container">
        <a class="navbar-brand" href="#">
          <img :src="require('@/assets/images/logo.png')" alt="" />
        </a>
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <router-link class="nav-link" to="/">Beranda</router-link>
            </li>
            <li class="nav-item dropdown">
              <b-nav-item-dropdown text="Fitur" left>
                <b-dropdown-item href="#">Cari Kampus/Prodi</b-dropdown-item>
                <b-dropdown-item href="#">Cari Event</b-dropdown-item>
                <b-dropdown-item href="#">Cari Beasiswa</b-dropdown-item>
                <b-dropdown-item href="#">Cari Magang</b-dropdown-item>
              </b-nav-item-dropdown>
            </li>
            <li class="nav-item">
              <a class="nav-link" aria-current="page" href="#">Hubungi Kami</a>
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="#">Blog</router-link>
            </li>
          </ul>
          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto">
            <ul class="navbar-nav me-auto mb-2 mb-lg-0 ml-auto">
              <li>
                <div class="btn">
                  <a class="nav-link" href="#"> <strong>Masuk</strong> </a>
                </div>
              </li>
              <li>
                <div class="btn btn-primary" id="daftar" >
                  <a class=" nav-link"  href="#">Daftar</a>
                </div>
                
              </li>
            </ul>
          </b-navbar-nav>
        </b-collapse>
      </div>
    </b-navbar>
  </div>
</template>

<script>
export default { name: "Navbar" };
</script>

<style>
</style>