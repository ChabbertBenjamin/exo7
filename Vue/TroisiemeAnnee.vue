<template>
    <view>
        <text>Troisieme Année</text>
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
