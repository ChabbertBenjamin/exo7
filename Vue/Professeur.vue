<template>
    <view>
        <text>Professeur</text>
        <button title="Retour" :on-press="() => navigation.goBack()"/>
    </view>
</template>



<script>
export default {
     props: {
    navigation: {
      type: Object
    }
  },
}
</script>



<style>
</style>
