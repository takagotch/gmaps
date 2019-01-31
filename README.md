### gmaps
---
https://github.com/HPNeo/gmaps

```js
var map = new GMaps({
  el: '#map',
  lat: -12.043333,
  lng: -77.028333
});

require.config({
  paths: {
    "googlemapapi": "googlemapapi",
  },
  shim: {
    gmaps: {
      deps: ["googlemapsapi"],
      exports: "GMaps"
    }
  }
});

define(['async!http://maps.google.com/maps/api/js?v=3&sensor=false'], function(){});
```

```css
#map {
  width: 400px;
  height: 400px
}
```

```
npm install
grunt
```

