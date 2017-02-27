[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/jifalops/geo-codec)

# geo-codec
Easily do geocoding and reverse geocoding with the Google maps API.

## Installation
```
bower install --save geo-codec
```

## Usage
You will need your own Google Maps API key to use this element. See the demo.

## Demo
<!--
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="geo-codec.html">
    <next-code-block></next-code-block>   
    <script>
      var codec = document.getElementById('codec');
      var search = document.getElementById('search');
      var results = document.getElementById('results');
      function runDemo() {      
        codec.geocode(search.value, function (address, lat, lng, place) {
          results.innerHTML = 'address: ' + address
            + '<br>lat: ' + lat
            + '<br>lng: ' + lng
            + '<br>placeId: ' + place;
        });
      }    
    </script>
  </template>
</custom-element-demo>
```
-->

```html
<geo-codec id="codec" api-key="AIzaSyAUPOaJubJnaRTPUd_xX8MOA62gRtSlfCc"></geo-codec>
<input id="search" /><button onclick="runDemo()">Search</button>
<div id="results"></div>
```

## Contributing

1. Fork it on Github.
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

## License

[MIT](https://opensource.org/licenses/MIT)
