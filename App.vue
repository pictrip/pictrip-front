<template>
    <app-navigation></app-navigation>
</template>

<script>
// import React from "react";
import { StackNavigator } from "vue-native-router";
// import HomeScreen from "../src/screens/homeScreen.vue";
// import DetailsScreen from "../src/screens/detailsScreen.vue";
import AppSignup from './src/screens/signup/index.vue';

const AppNavigation = StackNavigator(
  {
    Singup: AppSignup,
  },
  {
    initialRouteName: 'Singup',
  }
);
export default {
    components: { AppNavigation }
}
</script>
