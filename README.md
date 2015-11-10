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
