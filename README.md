# jQuery Geography   

## Structure   
```
o
|-- dist
|   |-- jquery-geography-google.js
|   `-- jquery-geography-google.min.js
|-- CHANGELOG
|-- LICENSE
`-- README.md
```

## Installation   
```
<script src="jquery.js"></script>
<script src="jquery-geography-google.min.js"></script>
```

## Usage   
```
<section class="map-area">
    <div class="map-content">
        <div class="map-initialize" style="background-image: url(assets/img/map/map-standard.jpg);"></div>
        <div class="map-responsive">
            <div class="map map-google"></div>
        </div>
    </div>
</section>
```
```
$('.map-google').geography();
```

## Example   

### Simple Example   

```
$('.map-google').geography();
```

### Example with options   
```
$('.map-google').geography({
    google: {
        api: {
            uri: 'https://maps.googleapis.com/maps/api/js',
            key: '', // API KEY
            language: 'en',
            region: 'AU'
        },
        map: {
            zoom: 12
        }
    }
});
```

### Example with data-attribute   
```
<section class="map-area">
    <div class="map-content">
        <div class="map-initialize" style="background-image: url(assets/img/map/map-retro.jpg);"></div>
        <div class="map-responsive">
            <div class="map map-google" data-geography-google='{"zoom":12,"styleWizard":"retro"}'></div>
        </div>
    </div>
</section>
```
```
<script>
    $('.map-google').geography();
</script>
```

## Changelog   
Please see [CHANGELOG](CHANGELOG) for more information what has changed recently.


## License   
jQuery Geography is licensed under the [MIT LICENSE](LICENSE)   
