<template>
  <div class="wrapper">
    <Navbar />

    <div class="jumbotron">
      <div class="container pt-5 mt-5">
        <div class="row" id="on-jumbotron">
          <div class="col-md-7 tagline">
            <h1 class="mb-3">
              <strong>Bingung Cari Informasi Seputar Kuliah ?</strong>
            </h1>
            <h3 class="mb-3">Cari disini aja!</h3>
            <h5 class="mb-4">
              Dapatkan informasi seputar dunia perkuliahan secara terupdate dari
              kami melalui aplikasi kampus indonesia
            </h5>
          </div>
          <div class="col-md-5" id="hero">
            <img
              class="img-fluid"
              src="../assets/images/hero.png"
              width="400px "
              alt=""
            />
          </div>
        </div>
        <div class="row d-flex justify-content-center">
          <div class="input-group mt-3 mb-3" id="cari">
            <input
              type="text"
              class="form-control"
              placeholder="Informasi seputar perkuliahan / Cari Kampus"
            />
            <button
              class="btn btn-outline-secondary"
              type="button"
              id="button-addon2"
            >
              <i class="fa fa-search"></i>
            </button>
          </div>
        </div>
      </div>
      <svg
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 1440 320"
        id="vector"
      >
        <path
          fill="#fff"
          fill-opacity="1"
          d="M0,160L120,176C240,192,480,224,720,213.3C960,203,1200,149,1320,122.7L1440,96L1440,320L1320,320C1200,320,960,320,720,320C480,320,240,320,120,320L0,320Z"
        ></path>
      </svg>
    </div>

    <!-- start best kampus -->
    <div class="container text-center">
      <div class="row">
        <div class="col text-center tagline">
          <h2>Rekomendasi <strong>Kampus Terbaik</strong></h2>
          <a href="" class="float-right btn btn-primary"
            >Lihat selengkapnya <i class="fa fa-caret-right ml-1"></i
          ></a>
        </div>
      </div>
      <hr /> 
          <CardUniv />
    </div>
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
      <path
        fill="#17a2af"
        fill-opacity="1"
        d="M0,0L48,32C96,64,192,128,288,165.3C384,203,480,213,576,192C672,171,768,117,864,101.3C960,85,1056,107,1152,106.7C1248,107,1344,85,1392,74.7L1440,64L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"
      ></path>
    </svg>
    <!-- end best kampus -->

    <!-- start fitur -->
    <div class="wrapper-fitur">
      <div class="container">
        <div class="row mb-4">
          <div class="col text-center">
            <h2 id="white-title"><strong>Fitur </strong>Kampus Indonesia</h2>
          </div>
        </div>

            <Fitur  />

      </div>
    </div>
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
      <path
        fill="#17a2af"
        fill-opacity="1"
        d="M0,32L48,64C96,96,192,160,288,160C384,160,480,96,576,96C672,96,768,160,864,165.3C960,171,1056,117,1152,90.7C1248,64,1344,64,1392,64L1440,64L1440,0L1392,0C1344,0,1248,0,1152,0C1056,0,960,0,864,0C768,0,672,0,576,0C480,0,384,0,288,0C192,0,96,0,48,0L0,0Z"
      ></path>
    </svg>
    <!-- end fitur -->
    <!-- start JobSeeker -->
    <div v-scrollanimation class="container mb-5">
      <div class="row">
        <div class="col-md-6">
          <img src="../assets/images/hero2.svg" width="400px" alt="" />
        </div>
        <div class="col-md-6 px-0 text-center">
          <h4 class="tagline">Apakah Kamu Sedang Mencari Pekerjaan ?</h4>
          <h5 class="tagline">Temukan Pekerjaan Terbaik Mu Disini</h5>
          <a class="btn btn-primary mt-3" href="">Click Disini</a>
        </div>
      </div>
    </div>
    <!-- end JobSeeker -->
    
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
      <path
        fill="#67ade7"
        fill-opacity="1"
        d="M0,0L48,32C96,64,192,128,288,165.3C384,203,480,213,576,192C672,171,768,117,864,101.3C960,85,1056,107,1152,106.7C1248,107,1344,85,1392,74.7L1440,64L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"
      ></path>
    </svg>
    <div class="container-artikel">
      <div class="container py-5 shadow" id="artikel">
        <div class="row">
          <div class="col mb-3 border-bottom artikel-tagline">
            <h2 style="color: #14375e"><strong>Artikel</strong> Terbaru</h2>
            <h5 style="color: #14375e">
              Jangan Sampai terlewat informasi terbaru kampus favoritmu
            </h5> <a href="" class="btn btn-primary float-right mr-4 mb-3 d-inline">Lihat selengkapnya</a>
            <!-- <hr class="mr-4" /> -->
          </div>
        </div>
        <div class="container">
          <carousel
            :nav="false"
            :items="4"
            :mouseDrag="true"
            :dots="true"
            :margin="-150"
            :responsive="{ 0: { items: 1, nav: false }, 600: { items: 3 } }"
          >
            <CardArtikel />
            <CardArtikel />
            <CardArtikel />
            <CardArtikel />
            <CardArtikel />
            <CardArtikel />
            <CardArtikel />
            <CardArtikel />
          </carousel>
        </div>
      </div>
    </div>
    

    <!-- Footer -->
    <Footer />
  </div>
</template>

    
<script>
// @ is an alias to /src
import Navbar from "@/components/Navbar.vue";
import Fitur from "@/components/Fitur.vue";
import CardUniv from "@/components/CardUniv.vue";
import CardArtikel from "@/components/CardArtikel.vue";
import Footer from "@/components/Footer.vue";
// import axios from "axios";
import $ from "jquery";
import carousel from "vue-owl-carousel";

export default {
  name: "Home",
  components: {
    Navbar,
    CardUniv,
    Fitur,
    carousel,
    CardArtikel,
    Footer,
  },
  data() {
    return {

    };
  },
  methods: {
    setUniversitas(data) {
      this.universitas = data;
    },
    setFitur(data) {
      this.fiturs = data;
    },
  },
  mounted() {
    // axios
    //   .get("http://localhost:3000/BestUniversitas")
    //   .then((response) => {
    //     // handle success
    //     console.log("Berhasil :", response);
    //     this.setUniversitas(response.data);
    //   })
    //   .catch((error) => {
    //     // handle error
    //     console.log(error);
    //   });
    // axios
    //   .get("http://localhost:3000/fitur")
    //   .then((response) => {
    //     // handle success
    //     console.log("Berhasil :", response);
    //     this.setFitur(response.data);
    //   })
    //   .catch((error) => {
    //     // handle error
    //     console.log(error);
    //   });
    this.$nextTick(() => {
      $(".jumbotron").fadeIn("slow");
    });
  },
};
</script>


<style>
.before-enter{
  opacity: 0;
  transform: translateY(100px);
  transition: all 2s ease-out;
}
.enter{
  opacity: 1;
  transform: translateY(0px);
}
</style>


