# Vue Skycons
Easily use [Skycons](https://github.com/darkskyapp/skycons) in your VueJs apps.

## Installation   
### NPM   
```
npm install --save vue-skycon
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
