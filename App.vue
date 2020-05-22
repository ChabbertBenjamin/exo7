<template>
  <app-navigator></app-navigator>
</template>

<script>
import {
  createAppContainer,
  createStackNavigator,
} from "vue-native-router";

import MainScreen from "./Vue/Main";
import PremiereAnneeScreen from "./Vue/PremiereAnnee";
import DeuxiemeAnneeScreen from "./Vue/DeuxiemeAnnee";
import TroisiemeAnneeScreen from "./Vue/TroisiemeAnnee";
import ProfesseurScreen from "./Vue/Professeur";


const StackNavigator = createStackNavigator(
  {
    Main: MainScreen,
    PremiereAnnee : PremiereAnneeScreen,
    DeuxiemeAnnee : DeuxiemeAnneeScreen,
    TroisiemeAnnee : TroisiemeAnneeScreen,
    Professeur : ProfesseurScreen,
  },
  {
    initialRouteName: 'Main',
  }
);

const AppNavigator = createAppContainer(StackNavigator);

export default {
  components: { AppNavigator },
}
</script>