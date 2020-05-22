<template>
    
  <view class="container" ref="app">

    <button
        :on-press="PageAccueil"
        title="Accueil"
        color="#8415CC"
    />
    <button
        :on-press="PagePremiereAnnee"
        title="Première Année"
        color="#8415AA"
    />
    <button
        :on-press="PageDeuxiemeAnnee"
        title="Deuxième Année"
        color="#841588"
    />
    <button
        :on-press="PageTroisiemeAnnee"
        title="Troisième Année"
        color="#841566"
    />
    <button
        :on-press="PageProfesseur"
        title="Professeur"
        color="#841544"
    />

        <touchable-opacity :on-press="PageAccueil">
            <image :source="require('../logo_exo7.png')"/>
        </touchable-opacity>
 
  </view>
</template>

<script>

import Menu from "./Menu";

export default {
    props: {
        navigation: {
            type: Object
        }
    }, 
    components: { Menu },
    methods:{
        PageAccueil(){
            this.navigation.navigate('Accueil')
        },
        PagePremiereAnnee(){
            this.navigation.navigate('PremiereAnnee')
        },
        PageDeuxiemeAnnee(){
            this.navigation.navigate('DeuxiemeAnnee')
        },
        PageTroisiemeAnnee(){
            this.navigation.navigate('TroisiemeAnnee')
        },
        PageProfesseur(){
            this.navigation.navigate('Professeur')
        },
    }
}
</script>
