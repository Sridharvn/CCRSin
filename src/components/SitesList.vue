<template>
  <div>
    <!-- <hr /> -->
    <h1>Our Upcoming Conference</h1>
    <div class="upComingEvent">
      <div class="siteslist__list">
        <a :href="sitesList[0].address" class="siteslist__link" target="_blank"
          ><v-img
            :src="require(`@/assets/${sitesList[0].image}`)"
            class="siteslist__image"
          ></v-img>
          <!-- <h3 class="siteslist__title">{{ sitesList[0].title }}</h3> -->
        </a>
      </div>
      <div class="upComingEventDetails">
        <h2>Oncology 2024</h2>
        <h3 class="">{{ sitesList[0].title }}</h3>
        <h3>March 8, 9 and 10 at Le Meridien, Kochi</h3>
        <h3>
          <a href="mailto:oncology2024@gmail.com">
            Email: oncology2024@gmail.com</a
          >
          <br />
          <a href="http://www.oncology2024.in/">Web: www.oncology2024.in</a>
        </h3>
      </div>
    </div>
    <br /><br />
    <h1>Official Websites of CCRS events from the past</h1>
    <div class="siteslist">
      <div
        v-for="(site, index) in sitesList"
        :key="site"
        class="siteslist__list"
      >
        <a :href="site.address" class="siteslist__link" v-if="index != 0"
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
  justify-content: center;
  //justify-content: space-evenly;
  align-items: flex-start;
  margin-top: 30px;
  gap: 20px;

  &__image {
    height: 210px;
    width: 435px;
    object-fit: cover;
    border-radius: 10px;
    margin: 10px;
    box-shadow: 0px 11px 15px -7px rgba(0, 0, 0, 0.2),
      0px 24px 38px 3px rgba(0, 0, 0, 0.14),
      0px 9px 46px 8px rgba(0, 0, 0, 0.12);
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
    width: 270px;
  }
}
.upComingEvent {
  background-color: #c2c3c5;
  padding: 10px;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  flex-wrap: wrap;
  .upComingEventDetails {
    display: flex;
    flex-direction: column;
    text-align: center;
    // color: white !important;
    a {
      text-decoration: none;
      color: black;
    }
  }
}
@media only screen and (max-width: 768px) {
  /* Styles here */
  .siteslist {
    &__image {
      height: 170px;
      width: 325px;

      &__link {
        margin: 30px;
        width: 300px;
      }

      &__list {
      }
      &__title {
        text-transform: capitalize;
        font-weight: 500;
        width: 250px;
      }
    }
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
            "INTERNATIONAL CONFERENCE ON MULTIDISCIPLINARY MANAGEMENT OF COMMON CANCERS - 2024",
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
        {
          address: "http://www.ccrsindia.in/oncology2003",
          title:
            "Association of Radiation Oncologists in India - 25th National Conference at Kochi - 2003",
          image: "sites/oncology2003.png",
        },
      ],
    };
  },
};
</script>
