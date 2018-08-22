<template>
    <!-- <app-navigation></app-navigation> -->
    <view class="signup">
        <text>Sample text</text>
        <text-input
            :style="inputStyle"
            placeholder="Enter your email"
            v-model="email"
        />
        <button
        :on-press="onPress"
        title="Signup"
        color="#fff"
        accessibility-label="Learn more about this purple button"
        />
    </view>
</template>

<script>
// import React from "react";
// import { StackNavigator } from "vue-native-router";
// import AppSignup from './src/screens/signup/index.vue';

// const AppNavigation = StackNavigator(
//   {
//     Singup: AppSignup,
//   },
//   {
//     initialRouteName: 'Singup',
//   }
// );
export default {
    // components: { AppNavigation }
    data() {
    return {
        email: '',
        inputStyle: {
            height: 40,
            width: 200, 
            borderColor: 'gray', 
            borderWidth: 1,
            borderRadius: 10,
            backgroundColor: 'rgba(255,255,255, 0.8)',
            marginTop: 10,
            padding: 15
        }
    }
  },
  methods: {
    onPress() {
        alert(`You entered ${this.email}`)
    }
  }
}
</script>

<style scoped>
.signup {
    background-color: #A83279;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
}
</style>