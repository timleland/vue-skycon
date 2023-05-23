# Vue Skycons
Easily use [Skycons](https://t.ly/_ic0) in your VueJs apps. Example use [Weather Extension](https://weatherextension.com/) and [WeatherTab](https://timleland.com/weathertab/)

<a href="https://www.digitalocean.com/?refcode=95e54284e826&utm_campaign=Referral_Invite&utm_medium=Referral_Program&utm_source=badge"><img src="https://web-platforms.sfo2.cdn.digitaloceanspaces.com/WWW/Badge%201.svg" alt="DigitalOcean Referral Badge" /></a>

## Installation   
### NPM   
```
npm i vue-skycon
```

### YARN   
```
yarn add vue-skycon
```

## Installation
```
import Vue from 'vue'
import VueSkycons from 'vue-skycon'

Vue.use(VueSkycons)

```

## Usage
```
<template>
  <div>
    <!-- General usage -->
    <skycon condition="clear-day" width="40" height="40"></skycon>
    <skycon condition="clear-night" width="40" height="40"></skycon>
    <skycon condition="partly-cloudy-day" width="40" height="40"></skycon>
    <skycon condition="partly-cloudy-night" width="40" height="40"></skycon>
    <skycon condition="cloudy" width="40" height="40"></skycon>
    <skycon condition="rain" width="40" height="40"></skycon>
    <skycon condition="sleet" width="40" height="40"></skycon>
    <skycon condition="snow" width="40" height="40"></skycon>
    <skycon condition="wind" width="40" height="40"></skycon>
    <skycon condition="fog" width="40" height="40"></skycon>
  </div>
</template>
```

## Props
```
  // Icon size
  width: {
    type: Number,
    default: 64
  },

  height: {
    type: Number,
    default: 64
  },

  color: {
    type: String,
    default: 'black'
  },

  // Weather condition
  condition: {
    type: String
  }
```
