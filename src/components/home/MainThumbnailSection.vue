<template>
  <div class="gallery">
    <figure class="gallery_item gallery_item--1">
      <img src="../../assets/images/Thumbnail5_Large.jpg" class="gallery_img" alt="Image 1">
    </figure>
    <figure class="gallery_item gallery_item--2">
      <img src="../../assets/images/chairs-2181968_1920.jpg" class="gallery_img" alt="Image 2">
    </figure>
    <figure class="gallery_item gallery_item--3">
      <img src="../../assets/images/Thumbnail3_Large.jpg" class="gallery_img" alt="Image 3">
    </figure>
  </div>
</template>

<script>
export default {
  name: 'MainThumbnails',
}
</script>

<style lang="scss" scoped>
.gallery {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  //grid-template-rows: repeat(8, 5vw);
  grid-gap: 0px;
}
.gallery_img {
  width: 100%;
  max-height: calc(100vh - 0rem - 7.7rem);
  height: 100%;
  object-fit: cover;
}
.gallery_item--1 {
  grid-column-start: 1;
  grid-column-end: 2;
  //grid-row-start: 1;
  //grid-row-end: 9;
}
.gallery_item--2 {
  grid-column-start: 2;
  grid-column-end: 3;
}
.gallery_item--3 {
  grid-column-start: 3;
  grid-column-end: 4;
}
figure {
  margin: 0;
}

</style>
