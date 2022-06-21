<template>
  <div id="home">
    <main>
      <h1>
        Cancer Control & Research Society (CCRS)
      </h1>
      
      <h3>Cancer Control & Research Society is a charitable organisation registered as per Act XII of 1955. The society is involved in cancer control activities by providing cancer care, palliative home care, assistance to suffering cancer patients, cancer awareness camps, continuing medical education programmes and international and national multidisciplinary oncology conferences.</h3>
      
      <br>
    </main>
    <aside>
      <img src="./../assets/317582_1100-732x549.jpg" alt="" style="max-height: 90vh; max-width: 55vw;" />
    </aside>
  </div>
</template>
<script>
</script>
<style scoped>
#home {
  display: flex;
  justify-content: space-between;
}

aside {
  display: flex;
}

main {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  flex-direction: column;
  padding: 10px;
}

#home {
  background-color: var(--primary-color);
  color: var(--secondary-color)
}

@media screen and (max-width: 800px) {
  #home {
    flex-direction: column;
  }

  aside {
    /* display: none; */
    /* ?justify center */
    justify-content: center;
    align-items: center;
    text-align: center;
    padding-bottom: 20px;
    /* width: max-content; */
  }

  h2 {
    font-size: 1.5rem;
    padding: 10px;
  }
}
</style>