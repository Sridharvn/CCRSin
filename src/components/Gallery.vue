<template>
  <div>
    <!-- https://drive.google.com/drive/folders/10xTO2aue9EQcS06hOyBCjifZXUkzKDen?usp=share_link -->

    <br />
    <!-- <Banner color="tertiary">Event Gallery</Banner> -->
    <img src="./../assets/EventGallery.jpeg" alt="Event Gallery" />
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
.galleryButton {
  @apply p-2 bg-text-primary2  text-white m-3 w-56 text-center rounded-lg transition-all mb-12 mt-6 font-bold text-xl;
  @apply hover:bg-text-primary;
}
.galleryDayWrapper {
  @apply flex flex-col-reverse justify-center items-center;
}
.galleryImage img {
  @apply rounded-xl;
}
.galleryImages {
  @apply flex flex-wrap gap-5 justify-center items-center;
}
.galleryImageItem {
  @apply h-64 w-96;
  @apply max-sm:h-[230px] max-sm:w-[340px];
}
.galleryWrapper {
  @apply flex justify-center flex-col items-center  shadow-xl gap-12;
}
</style>
