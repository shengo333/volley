<template>
  <div class="indexPageWrapper">
    <slider/>

  </div>
</template>

<script>
import { mapState } from 'vuex';
import slider from '@/components/Theimgslider.vue';
import { onMounted } from 'vue';

export default {
  name: 'IndexPage',
  components: {
    slider,
  },
  methods:{
    checkLoggedIn() {
      console.log('we are here')
    if(localStorage.getItem('isLoggedIn') === 'true'){
      alert('user is logged in')
    } else{
      this.$router.push('/login');
      alert('გთხოვთ გაიაროთ ავტორიზაცია')
    }
    
  },
  },
  mounted(){
    this.checkLoggedIn()
  }
};
</script>

<style lang="scss">
/* Your styles here */
</style>