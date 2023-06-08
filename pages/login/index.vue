<template>
  <div>
    <div class="log-in">
          <input type="text" placeholder="შეიყვანე იუზერი" v-model="userName">
          <input type="text" placeholder="შეიყვანე პაროლი" v-model="password">
          <button @click="logIn"> log in</button>
      </div>
    <nuxt />
  </div>
</template>

<script>
export default {

  data(){
    return{
      userName: '',
      password: ''
    }
  },
  methods:{
    logIn() {
      console.log('something')
      // Check if name and password are valid (any values for demonstration purposes)
      if (this.userName.length > 0 && this.password.length > 0) {
        // Perform any additional validation or authentication here

        // Set login value to local storage
        localStorage.setItem('isLoggedIn', 'true');

        // Redirect to a new page after successful login
        this.$router.push('/');
      }
    },
  }


}
</script>

<style>

</style>