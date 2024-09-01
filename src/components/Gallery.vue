<template>
  <div>
    <!-- https://drive.google.com/drive/folders/10xTO2aue9EQcS06hOyBCjifZXUkzKDen?usp=share_link -->

    <br />
    <!-- <Banner color="tertiary">Event Gallery</Banner> -->
    <img
      src="./../assets/EventGallery.jpeg"
      alt="Event Gallery"
      class="headerImage"
    />
    <br />

    <div class="galleryWrapper">
      <div
        class="galleryDayWrapper"
        v-for="(item, index) in imageDirectory"
        :key="index"
      >
        <div class="galleryButton">
          <a :href="item.link" target="_blank">{{ item.day }}</a>
        </div>
        <div class="galleryImages">
          <div
            class="galleryImage"
            v-for="(image, index2) in item.images.slice(0, 15)"
            :key="index2"
          >
            <img
              :src="getImage(image)"
              :alt="getImage(image)"
              class="galleryImageItem"
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
// eslint-disable-next-line no-unused-vars
import imageDirectory from "./data/eventGallery.ts";

export default {
  data() {
    return {
      imageDirectory: imageDirectory,
    };
  },
  methods: {
    getImage(gDriveUrl) {
      let fileId = gDriveUrl.split("/")[5]; // Extracts the file ID from the URL
      return `https://drive.google.com/thumbnail?export=view&id=${fileId}`;
    },
  },
};
</script>
<style scoped>
* {
  /* outline: 1px solid red; */
}
/* .headerImage{ */
.headerImage {
  width: 100%;
  height: auto;
  max-width: fit-content;
}
/* } */
.galleryButton {
  padding: 0.5rem;
  background-color: #2b6cb0;
  color: #fff;
  margin: 0.75rem;
  width: 14rem;
  text-align: center;
  border-radius: 0.5rem;
  transition: all 0.3s;
  font-weight: bold;
  font-size: 1.5rem;
}
a {
  text-decoration: none;
  color: white !important;
}

.galleryButton:hover {
  background-color: #3182ce;
}

.galleryDayWrapper {
  display: flex;
  flex-direction: column-reverse;
  justify-content: center;
  align-items: center;
}

.galleryImage img {
  border-radius: 0.5rem;
  width: 80%;
}

.galleryImages {
  display: flex;
  flex-wrap: wrap;
  gap: 1.25rem;
  justify-content: center;
  align-items: center;
}

.galleryImageItem {
  height: 16rem;
  width: 24rem;
  max-height: 230px;
  max-width: 340px;
}

.galleryWrapper {
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  box-shadow: 0 0.25rem 0.5rem rgba(0, 0, 0, 0.15);
  gap: 3rem;
}

@media (max-width: 640px) {
  .galleryButton {
    width: 10rem;
  }

  .galleryImageItem {
    height: 12rem;
    width: 18rem;
    max-height: 180px;
    max-width: 280px;
  }
}
</style>
