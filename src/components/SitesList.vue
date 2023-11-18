<template>
  <div>
    <br /><br />
    <h1>Official Websites of CCRS events from the past</h1>
    <div class="siteslist">
      <div v-for="site in sitesList" :key="site" class="siteslist__list">
        <a :href="site.address" class="siteslist__link"
          ><v-img
            :src="require(`@/assets/${site.image}`)"
            class="siteslist__image"
          ></v-img>
          <h3 class="siteslist__title">{{ site.title }}</h3>
        </a>
      </div>
    </div>
  </div>
</template>
<style lang="scss" scoped>
.siteslist {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-evenly;
  align-items: center;
  margin-top: 30px;

  &__image {
    height: 210px;
    width: 435px;
    object-fit: cover;
    border-radius: 10px;
    margin: 10px;
  }

  &__link {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-decoration: none;
    color: var(--text-color);
    margin: 30px;
    width: 433px;
    text-align: center;
  }

  &__list {
  }

  &__title {
    text-transform: capitalize;
    font-weight: 500;
  }
}
</style>
<script>
export default {
  data() {
    return {
      sitesList: [
        {
          address: "http://www.oncology2024.in",
          title:
            "International Conference on Recent Advances in the Multidisciplinary Management of Common Malignancies - 2022",
          image: "sites/oncology2024.png",
        },
        {
          address: "http://www.ccrsindia.in/oncology2022",
          title:
            "International Conference on Recent Advances in the Multidisciplinary Management of Common Malignancies - 2022",
          image: "sites/oncology2022.png",
        },
        {
          address: "http://www.ccrsindia.in/oncology2018",
          title:
            "International conference on multidisciplinary management of common cancers - 2018",
          image: "sites/oncology2018.png",
        },
        {
          address: "http://www.ccrsindia.in/oncology2014",
          title:
            "international conference on multidisciplinary management of breast cancer - 2014",
          image: "sites/oncology2014.png",
        },
        {
          address: "http://www.ccrsindia.in/oncology2012",
          title:
            "international conference on multidisciplinary management of common cancers - 2012",
          image: "sites/oncology2012.png",
        },
        {
          address: "http://www.ccrsindia.in/oncology2009",
          title: "Oncology conference with international participation - 2009",
          image: "sites/oncology2009.png",
        },
      ],
    };
  },
};
</script>
