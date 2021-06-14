<template>
<div style="display: inline-flex">
  <div class="row">
    <div class="col-md-6 px-0" v-for="(fitur, index) in fiturs" :key="index">
      <a href="#" style="text-decoration: none">
  <div class="card" style="width: 100%;" id="wrapperfitur">
    <div class="card-body fitur-body p-0 " :id="fitur.fitur">
      <p class="card-text text-center title-fitur" >{{ fitur.title }}</p>
    </div>
  </div>
      </a>

    </div>
  </div>
</div>

</template>

<script>
export default {
  name: "Fitur",

  data(){
    return{
      fiturs:[
        {
        "id":1,
        "fitur":"fitur1",
        "title" : "Kampus"
      },
      {
        "id":2,
        "fitur":"fitur2",
        "title" : "Beasiswa"
      },
      {
        "id":3,
        "fitur":"fitur3",
        "title" : "Seminar/Workshop"
      },
      {
        "id":4,
        "fitur":"fitur4",
        "title" : "UTBK"
      },
      {
        "id":5,
        "fitur":"fitur5",
        "title" : "Lowongan"
      },
      {
        "id":6,
        "fitur":"fitur6",
        "title" : "Lomba"
      }
      ]
    }
  }
};
</script>

<style>
.fitur {
  max-width: 100%;
  border: none;

  object-fit: cover;
  /* object-fit:scale-down; */
}

#wrapperfitur {
  border: none;
  border-radius: 0;
}

.fitur-body {
  height: 300px;
  transition: 0.3s;
}

.fitur-body:hover {
  opacity: 0.9;
  text-shadow: 3px 2px 6px rgba(0, 0, 0, 0.8);
  font-size: 20px;
}
</style>
