<template>
  <div>
    <a
      href="http://www.cybernetdevelopers.com"
      target="_blank"
      class="cyDevLink"
      ><div class="cyDevText">Web Design by</div>
      <span
        ><img src="@/assets/logotoptransparent.png" alt="" class="cyDevLogo"
      /></span>
    </a>
  </div>
</template>
<style scoped>
div {
  background: #000;
  color: white;
  display: flex;
  justify-content: flex-end;
  padding-block: 4px;
}
a {
  display: flex;
  gap: 10px;
  text-decoration: none;
  align-items: center;
  padding-inline: 10px;
  font-family: "Roboto Condensed", sans-serif;
}
img {
  height: 20px;
  width: 20px;
  opacity: 0.9;
  transform: translateY(2px);
}
</style>
