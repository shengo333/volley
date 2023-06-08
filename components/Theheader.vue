<template>
  <div class="headerWrapper">
    <div class="leftHeader">
      <div class="icon">icon</div>



    </div>
    <div class="navbar">
      <!-- <ul>
            <li v-for="botton in bottons"></li>
        </ul> -->
      <ul>
        <nuxt-link :to="{name: 'index'}">
          <li>მთავარი</li>
        </nuxt-link>
        <nuxt-link :to="{name: 'federation'}">
          <li>ფედერაცია</li>
        </nuxt-link>
        <nuxt-link :to="{name: 'news'}">
          <li>სიახლეები</li>
        </nuxt-link>
        <nuxt-link :to="{name: 'nationalTeam'}">
          <li>ეროვნული გუნდი</li>
        </nuxt-link>
        <nuxt-link :to="{name: 'clubs-clubs'}">
          <li>კლუბები</li>
        </nuxt-link>
        <nuxt-link :to="{name: 'calendar'}">
          <li>კალენდარი</li>
        </nuxt-link>
        <nuxt-link :to="{name: 'contact'}">
          <li>კონტაქტი</li>
        </nuxt-link>
        <nuxt-link :to="{name: 'login'}">
          <li>ავტორიზაცია</li>
        </nuxt-link>
      </ul>
    </div>
  </div>
</template>

<script>
export default {

  




};
</script>

<style lang="scss" scoped>

.log-in{
  display: flex;
}

.headerWrapper {
  background: #3f4267;
  height: 10vh;
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  .navbar{
    width: 80%;
    display: flex;
    align-items: center;
    justify-content: flex-end;
      ul{
        display: flex;
        align-items: center;
        gap: 1rem;
        margin: 0;
          li {
            list-style-type: none;
            color: white;
          }
      }
  }
}
</style>