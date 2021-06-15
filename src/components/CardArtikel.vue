<template>
  <div class="card" style="width: 18rem;">
  <img class="card-img-top img-artikel" src="https://placeimg.com/200/200/any?1" alt="Card image cap">
  <div class="card-body">
    <p class="card-text" style="color:black">Judul Artikel Terbaru Kampus Indonesia</p>
    <a href="#" class="btn btn-primary">Baca Selengkapnya</a>
  </div>
</div>
</template>

<script>
export default {
  name: "CardArtikel",
  props:
    ['artikel']
};
</script>

<style>
.img-artikel{
    height: 200px;
    object-fit: cover;
}
.card{
    border: 2px solid black;
}
</style>