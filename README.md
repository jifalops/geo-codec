[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/jifalops/geo-codec)

# geo-codec
Easily geocode and reverse geocode strings and coordinates.

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
      var return1 = document.getElementById('return');
      var results = document.getElementById('results');
      function runDemo() {
        var ret = codec.geocode(search.value, function (address, lat, lng, place) {
          results.innerHTML = 'address: ' + address
            + '<br>lat: ' + lat
            + '<br>lng: ' + lng
            + '<br>placeId: ' + place;
        });
        if (ret) return1.innerText = 'Sent to geocoder.';
        else if (ret === null) return1.innerText = 'Geocoder will use when ready.';
        else if (ret === false) return1.innerText = 'Result was cached.';
      }
    </script>
  </template>
</custom-element-demo>
```
-->

```html
<geo-codec id="codec" api-key="AIzaSyAUPOaJubJnaRTPUd_xX8MOA62gRtSlfCc"></geo-codec>
<input id="search" /><button onclick="runDemo()">Search</button>
<div id="return"></div>
<div id="results"></div>
```

Full demo:
[webcomponents.org](https://www.webcomponents.org/element/jifalops/geo-codec/demo/demo/index.html)
| [github](https://jifalops.github.io/geo-codec/components/geo-codec/demo/).

API: [webcomponents.org](https://www.webcomponents.org/element/jifalops/geo-codec/geo-codec)
| [github](https://jifalops.github.io/geo-codec).

## Contributing

1. Fork it on Github.
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

## License

[MIT](https://opensource.org/licenses/MIT)
