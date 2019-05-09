# jQuery Geography   

## Demo   
[Demo](https://krescentmoon.github.io/jquery-geography/)   


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


## Options   
```
| map       | feature   | property              | type      | value                                                         |
|--------   |---------  |-------------------    |---------  |-------------------------------------------------------------  |
| google    | api       | uri                   | string    | 'https://maps.googleapis.com/maps/api/js'                     |
| google    | api       | key                   | string    | ''                                                            |
| google    | api       | language              | string    | 'en'                                                          |
| google    | api       | region                | string    | 'AU'                                                          |
| google    | map       | lat                   | number    | -34.397                                                       |
| google    | map       | lng                   | number    | 150.644                                                       |
| google    | map       | zoom                  | number    | 8                                                             |
| google    | map       | icon                  | string    | ''                                                            |
| google    | map       | draggable             | boolean   | true                                                          |
| google    | map       | scrollwheel           | boolean   | false                                                         |
| google    | map       | styleWizard           | string    | 'standard','silver','retro','dark','night','aubergine'        |
| google    | map       | zoomControl           | boolean   | true                                                          |
| google    | map       | mapTypeControl        | boolean   | false                                                         |
| google    | map       | scaleControl          | boolean   | false                                                         |
| google    | map       | streetViewControl     | boolean   | false                                                         |
| google    | map       | rotateControl         | boolean   | false                                                         |
| google    | map       | fullscreenControl     | boolean   | false                                                         |
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
            <div class="map map-google" data-geography-google='{"lat":-34.397,"lng":150.644,"icon":"","styleWizard":"retro"}'></div>
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
