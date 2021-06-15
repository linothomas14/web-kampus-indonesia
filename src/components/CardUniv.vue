<template>
  <div style="display: inline-flex">
    <div class="row my-4">
    <div class="col-md-3" v-for="(univ, index) in universitas" :key="index">
      <div class="card shadow card-univ pt-4 mb-2 " >
        <div class="btn" id="love"><i class="fa fa-heart"></i></div>
        <img
          class="card-img-top img-univ mx-auto"
          :src="require(`@/assets/images/${univ.gambar}`)"
          alt="Card image cap"
        /> 

        <div class="card-body">
          <h5 class="card-title">{{ univ.nama }}</h5>

          <router-link to="/" class="btn" id="CardUniv"
            >Lihat detail <i class="fa fa-chevron-right"></i
          ></router-link>
        </div>
      </div>
    </div>
        </div>
  </div>
</template>

<script>


export default {
  name: "CardUniv",
  props: ["listdata"],
  data(){
    return{
      universitas: [
        {
        "id": 1,
        "nama": "Universitas Indonesia",
        "gambar": "ui.png"
      },
      {
        "id": 2,
        "nama": "Institut Teknologi Bandung",
        "gambar": "itb.png"
      },
      {
        "id": 3,
        "nama": "Institut Pertanian Bogor",
        "gambar": "ipb.png"
      },
      {
        "id": 4,
        "nama": "Universitas Gundarma",
        "gambar": "gunadarma.png"
      },

      ],
    }
  },
  
};
</script>

<style>

#CardUniv {
  background-color: #1756af;
  color: #ffffff;
  border-radius: 7px;
}

#CardUniv:hover {
  background-color: #1a4075;
  color: white;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
}

#love {
  color: red;
  box-shadow: 0px 2px 10px 3px rgba(0, 0, 0, 0.1);
  position: absolute;
  right: 10px;
  top: 10px;
  border-radius: 20px;
}




</style>