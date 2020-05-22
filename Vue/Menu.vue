<template>
  <view>
    <text>MENU TEST</text>
    <button title="Première année" @press="PagePremiereAnnee"></button>
    <text>___________</text>
  </view>
</template>

<script>


export default {
  props: {
      navigation: {
        type: Object
      }
  }, 
  methods:{
    PagePremiereAnnee(){
      this.navigation.navigate('PremiereAnnee')

    }
  }
};
</script>