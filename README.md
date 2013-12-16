dolar-blue
==========

Client for the dolar-blue.net API in nodejs


## Synopsis

``` javascript
var dolarblue = require('dolar-blue');

dolarblue(function(data){
    console.log(data.datetime": el dolar blue esta a " + data.buy + " - " + data.sell);
    console.log("Debería comprar?");
});

```

## API

### dolarblue(callback(data))

*** callback *** 
    argument is an object with 3 members: buy, sell and datetime. Datetime's format is ISO8601 and is suitable for 
``` javascript
    var date = new Date(data.datetime);
```

## TODO
Support other sources of data.

## References
http://www.eldolarblue.net/dolar-blue-web-services.php
