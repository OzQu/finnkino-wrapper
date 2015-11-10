# finnkino-wrapper
Finnkino xml api wrapper. Should work with other Markus cinema systems API's also.
http://www.finnkino.fi/xml

## Usage
```
var fk = require('finnkino-wrapper');

// See valid options from http://www.finnkino.fi/xml
// Some endpoints are not even using the options.
var options = { };

fk.areas(options, function(result) {
    console.log(result);
});
fk.languages(options, function(result) {
    console.log(result);
});
fk.scheduleDates(options, function(result) {
    console.log(result);
});
fk.schedule(options, function(result) {
    console.log(result);
});
fk.events(options, function(result) {
    console.log(result);
});
fk.news(options, function(result) {
    console.log(result);
});
fk.newsCategories(options, function(result) {
    console.log(result);
});
// Default is set in code to http://www.finnkino.fi/xml
fk.setApiAddress('www.finnkino.fi/xml');
```

## Future
If and when I can find or create xml schema for finnkino API, xml-parser can do all the 'heavy' lifting which is now done almost manually and not necessary even correctly. At this point this more or less for my own usage and considers just my needs.
