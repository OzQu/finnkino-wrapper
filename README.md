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

## Example of response from finnkino.fi/xml/Schedule through this wrapper
```xml
<Show>
<ID>818142</ID>
<dtAccounting>2015-11-15T00:00:00</dtAccounting>
<dttmShowStart>2015-11-15T12:00:00</dttmShowStart>
<dttmShowStartUTC>2015-11-15T10:00:00Z</dttmShowStartUTC>
<dttmShowEnd>2015-11-15T13:32:00</dttmShowEnd>
<dttmShowEndUTC>2015-11-15T11:32:00Z</dttmShowEndUTC>
<ShowSalesStartTime>2000-01-01T00:00:00</ShowSalesStartTime>
<ShowSalesStartTimeUTC>2000-01-01T00:00:00Z</ShowSalesStartTimeUTC>
<ShowSalesEndTime>2015-11-15T11:45:00</ShowSalesEndTime>
<ShowSalesEndTimeUTC>2015-11-15T09:45:00Z</ShowSalesEndTimeUTC>
<ShowReservationStartTime>2000-01-01T00:00:00</ShowReservationStartTime>
<ShowReservationStartTimeUTC>2000-01-01T00:00:00Z</ShowReservationStartTimeUTC>
<ShowReservationEndTime>2015-11-15T10:30:00</ShowReservationEndTime>
<ShowReservationEndTimeUTC>2015-11-15T08:30:00Z</ShowReservationEndTimeUTC>
<EventID>301006</EventID>
<Title>Onnelin ja Annelin talvi</Title>
<OriginalTitle>Onnelin ja Annelin talvi</OriginalTitle>
<ProductionYear>2015</ProductionYear>
<LengthInMinutes>82</LengthInMinutes>
<dtLocalRelease>2015-10-09T00:00:00</dtLocalRelease>
<Rating>S</Rating>
<RatingLabel>S</RatingLabel>
<RatingImageUrl>
https://media.finnkino.fi/images/rating_large_S.png
</RatingImageUrl>
<EventType>Movie</EventType>
<Genres>Perhe-elokuva, Kotimainen</Genres>
<TheatreID>1037</TheatreID>
<TheatreAuditriumID>1232</TheatreAuditriumID>
<Theatre>Plevna, Tampere</Theatre>
<TheatreAuditorium>sali 1</TheatreAuditorium>
<TheatreAndAuditorium>Plevna, Tampere, sali 1</TheatreAndAuditorium>
<PresentationMethodAndLanguage>suomi</PresentationMethodAndLanguage>
<PresentationMethod/>
<EventSeries/>
<ShowURL>http://www.finnkino.fi/Websales/Show/818142/</ShowURL>
<EventURL>http://www.finnkino.fi/Event/301006/</EventURL>
<Images>
<EventMicroImagePortrait>
http://media.finnkino.fi/1012/Event_10344/portrait_micro/OnneliAnnelinTalvi_1080.jpg
</EventMicroImagePortrait>
<EventSmallImagePortrait>
http://media.finnkino.fi/1012/Event_10344/portrait_small/OnneliAnnelinTalvi_1080.jpg
</EventSmallImagePortrait>
<EventMediumImagePortrait>
http://media.finnkino.fi/1012/Event_10344/portrait_medium/OnneliAnnelinTalvi_1080.jpg
</EventMediumImagePortrait>
<EventLargeImagePortrait>
http://media.finnkino.fi/1012/Event_10344/portrait_small/OnneliAnnelinTalvi_1080.jpg
</EventLargeImagePortrait>
<EventSmallImageLandscape>
http://media.finnkino.fi/1012/Event_10344/landscape_small/OnneliAnnelinTalvi_444.jpg
</EventSmallImageLandscape>
<EventLargeImageLandscape>
http://media.finnkino.fi/1012/Event_10344/landscape_large/OnneliAnnelinTalvi_670.jpg
</EventLargeImageLandscape>
</Images>
<ContentDescriptors/>
</Show>
<Show>
<ID>818333</ID>
<dtAccounting>2015-11-15T00:00:00</dtAccounting>
<dttmShowStart>2015-11-15T12:00:00</dttmShowStart>
<dttmShowStartUTC>2015-11-15T10:00:00Z</dttmShowStartUTC>
<dttmShowEnd>2015-11-15T13:59:00</dttmShowEnd>
<dttmShowEndUTC>2015-11-15T11:59:00Z</dttmShowEndUTC>
<ShowSalesStartTime>2000-01-01T00:00:00</ShowSalesStartTime>
<ShowSalesStartTimeUTC>2000-01-01T00:00:00Z</ShowSalesStartTimeUTC>
<ShowSalesEndTime>2015-11-15T11:45:00</ShowSalesEndTime>
<ShowSalesEndTimeUTC>2015-11-15T09:45:00Z</ShowSalesEndTimeUTC>
<ShowReservationStartTime>2000-01-01T00:00:00</ShowReservationStartTime>
<ShowReservationStartTimeUTC>2000-01-01T00:00:00Z</ShowReservationStartTimeUTC>
<ShowReservationEndTime>2015-11-15T10:30:00</ShowReservationEndTime>
<ShowReservationEndTimeUTC>2015-11-15T08:30:00Z</ShowReservationEndTimeUTC>
<EventID>301266</EventID>
<Title>Louder Than Bombs</Title>
<OriginalTitle>Louder Than Bombs</OriginalTitle>
<ProductionYear>2015</ProductionYear>
<LengthInMinutes>109</LengthInMinutes>
<dtLocalRelease>2015-11-06T00:00:00</dtLocalRelease>
<Rating>12</Rating>
<RatingLabel>12</RatingLabel>
<RatingImageUrl>
https://media.finnkino.fi/images/rating_large_12.png
</RatingImageUrl>
<EventType>Movie</EventType>
<Genres>Draama</Genres>
<TheatreID>1037</TheatreID>
<TheatreAuditriumID>1247</TheatreAuditriumID>
<Theatre>Plevna, Tampere</Theatre>
<TheatreAuditorium>sali 5</TheatreAuditorium>
<TheatreAndAuditorium>Plevna, Tampere, sali 5</TheatreAndAuditorium>
<PresentationMethodAndLanguage>English/French</PresentationMethodAndLanguage>
<PresentationMethod/>
<EventSeries/>
<ShowURL>http://www.finnkino.fi/Websales/Show/818333/</ShowURL>
<EventURL>http://www.finnkino.fi/Event/301266/</EventURL>
<Images>
<EventMicroImagePortrait>
http://media.finnkino.fi/1012/Event_10605/portrait_micro/LouderThanBombs_1080.jpg
</EventMicroImagePortrait>
<EventSmallImagePortrait>
http://media.finnkino.fi/1012/Event_10605/portrait_small/LouderThanBombs_1080.jpg
</EventSmallImagePortrait>
<EventMediumImagePortrait>
http://media.finnkino.fi/1012/Event_10605/portrait_medium/LouderThanBombs_1080.jpg
</EventMediumImagePortrait>
<EventLargeImagePortrait>
http://media.finnkino.fi/1012/Event_10605/portrait_small/LouderThanBombs_1080.jpg
</EventLargeImagePortrait>
<EventSmallImageLandscape>
http://media.finnkino.fi/1012/Event_10605/landscape_small/LouderThanBombs_444f.jpg
</EventSmallImageLandscape>
<EventLargeImageLandscape>
http://media.finnkino.fi/1012/Event_10605/landscape_large/LouderThanBombs_670f.jpg
</EventLargeImageLandscape>
</Images>
<ContentDescriptors>
<ContentDescriptor>
<Name>Violence</Name>
<ImageURL>
https://media.finnkino.fi/images/content_Violence.png
</ImageURL>
</ContentDescriptor>
<ContentDescriptor>
<Name>Disturbing</Name>
<ImageURL>
https://media.finnkino.fi/images/content_Disturbing.png
</ImageURL>
</ContentDescriptor>
</ContentDescriptors>
</Show>
```
Xml above is parsed to following
```
[
  { ID: '818142',
    dtAccounting: '2015-11-15T00:00:00',
    dttmShowStart: '2015-11-15T12:00:00',
    dttmShowStartUTC: '2015-11-15T10:00:00Z',
    dttmShowEnd: '2015-11-15T13:32:00',
    dttmShowEndUTC: '2015-11-15T11:32:00Z',
    ShowSalesStartTime: '2000-01-01T00:00:00',
    ShowSalesStartTimeUTC: '2000-01-01T00:00:00Z',
    ShowSalesEndTime: '2015-11-15T11:45:00',
    ShowSalesEndTimeUTC: '2015-11-15T09:45:00Z',
    ShowReservationStartTime: '2000-01-01T00:00:00',
    ShowReservationStartTimeUTC: '2000-01-01T00:00:00Z',
    ShowReservationEndTime: '2015-11-15T10:30:00',
    ShowReservationEndTimeUTC: '2015-11-15T08:30:00Z',
    EventID: '301006',
    Title: 'Onnelin ja Annelin talvi',
    OriginalTitle: 'Onnelin ja Annelin talvi',
    ProductionYear: '2015',
    LengthInMinutes: '82',
    dtLocalRelease: '2015-10-09T00:00:00',
    Rating: 'S',
    RatingLabel: 'S',
    RatingImageUrl: 'https://media.finnkino.fi/images/rating_large_S.png',
    EventType: 'Movie',
    Genres: 'Perhe-elokuva, Kotimainen',
    TheatreID: '1037',
    TheatreAuditriumID: '1232',
    Theatre: 'Plevna, Tampere',
    TheatreAuditorium: 'sali 1',
    TheatreAndAuditorium: 'Plevna, Tampere, sali 1',
    PresentationMethodAndLanguage: 'suomi',
    PresentationMethod: '',
    EventSeries: '',
    ShowURL: 'http://www.finnkino.fi/Websales/Show/818142/',
    EventURL: 'http://www.finnkino.fi/Event/301006/',
    Images: 
     { EventMicroImagePortrait: 'http://media.finnkino.fi/1012/Event_10344/portrait_micro/OnneliAnnelinTalvi_1080.jpg',
       EventSmallImagePortrait: 'http://media.finnkino.fi/1012/Event_10344/portrait_small/OnneliAnnelinTalvi_1080.jpg',
       EventMediumImagePortrait: 'http://media.finnkino.fi/1012/Event_10344/portrait_medium/OnneliAnnelinTalvi_1080.jpg',
       EventLargeImagePortrait: 'http://media.finnkino.fi/1012/Event_10344/portrait_small/OnneliAnnelinTalvi_1080.jpg',
       EventSmallImageLandscape: 'http://media.finnkino.fi/1012/Event_10344/landscape_small/OnneliAnnelinTalvi_444.jpg',
       EventLargeImageLandscape: 'http://media.finnkino.fi/1012/Event_10344/landscape_large/OnneliAnnelinTalvi_670.jpg' },
    ContentDescriptors: '' },
  { ID: '818333',
    dtAccounting: '2015-11-15T00:00:00',
    dttmShowStart: '2015-11-15T12:00:00',
    dttmShowStartUTC: '2015-11-15T10:00:00Z',
    dttmShowEnd: '2015-11-15T13:59:00',
    dttmShowEndUTC: '2015-11-15T11:59:00Z',
    ShowSalesStartTime: '2000-01-01T00:00:00',
    ShowSalesStartTimeUTC: '2000-01-01T00:00:00Z',
    ShowSalesEndTime: '2015-11-15T11:45:00',
    ShowSalesEndTimeUTC: '2015-11-15T09:45:00Z',
    ShowReservationStartTime: '2000-01-01T00:00:00',
    ShowReservationStartTimeUTC: '2000-01-01T00:00:00Z',
    ShowReservationEndTime: '2015-11-15T10:30:00',
    ShowReservationEndTimeUTC: '2015-11-15T08:30:00Z',
    EventID: '301266',
    Title: 'Louder Than Bombs',
    OriginalTitle: 'Louder Than Bombs',
    ProductionYear: '2015',
    LengthInMinutes: '109',
    dtLocalRelease: '2015-11-06T00:00:00',
    Rating: '12',
    RatingLabel: '12',
    RatingImageUrl: 'https://media.finnkino.fi/images/rating_large_12.png',
    EventType: 'Movie',
    Genres: 'Draama',
    TheatreID: '1037',
    TheatreAuditriumID: '1247',
    Theatre: 'Plevna, Tampere',
    TheatreAuditorium: 'sali 5',
    TheatreAndAuditorium: 'Plevna, Tampere, sali 5',
    PresentationMethodAndLanguage: 'English/French',
    PresentationMethod: '',
    EventSeries: '',
    ShowURL: 'http://www.finnkino.fi/Websales/Show/818333/',
    EventURL: 'http://www.finnkino.fi/Event/301266/',
    Images: 
     { EventMicroImagePortrait: 'http://media.finnkino.fi/1012/Event_10605/portrait_micro/LouderThanBombs_1080.jpg',
       EventSmallImagePortrait: 'http://media.finnkino.fi/1012/Event_10605/portrait_small/LouderThanBombs_1080.jpg',
       EventMediumImagePortrait: 'http://media.finnkino.fi/1012/Event_10605/portrait_medium/LouderThanBombs_1080.jpg',
       EventLargeImagePortrait: 'http://media.finnkino.fi/1012/Event_10605/portrait_small/LouderThanBombs_1080.jpg',
       EventSmallImageLandscape: 'http://media.finnkino.fi/1012/Event_10605/landscape_small/LouderThanBombs_444f.jpg',
       EventLargeImageLandscape: 'http://media.finnkino.fi/1012/Event_10605/landscape_large/LouderThanBombs_670f.jpg' },
    ContentDescriptors: { ContentDescriptor: [Object] } }
]

```

## Future
If and when I can find or create xml schema for finnkino API, xml-parser can do all the 'heavy' lifting which is now done almost manually and not necessary even correctly. At this point this more or less for my own usage and considers just my needs.
