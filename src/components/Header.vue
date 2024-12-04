<template>
  <div v-if="!useris">
    <button  @click="signIn">Sign In</button>
  </div>
  <div v-else>
    <button  @click="signOut" >Sign Out</button>
    <button>Profile</button>

  </div>
</template>
<script>
export default {
  data() {
    return {
      useris: false
    }
  },
  methods:{
      signIn()
      {
        this.useris=true;
      },
      signOut()
      {
        this.useris=false;
      }
  }
}

</script>