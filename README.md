# ![LOGO](logo.png) NeoWs - (Near Earth Object Web Service) **flow**ground Connector

## Description

A generated **flow**ground connector for the NeoWs - (Near Earth Object Web Service) API (version 1.0).

Generated from: https://api.apis.guru/v2/specs/neowsapp.com/1.0/swagger.json<br/>
Generated at: 2019-05-07T17:43:12+03:00

## API Description

A web service for near earth objects. All the data is from the  <a href="http://neo.jpl.nasa.gov/" target="_blank">NASA JPL Asteroid team</a>. 

 

NeoWs is proud to power AsteroidTracker on <a href="https://itunes.apple.com/us/app/asteroid-tracker/id689684901?mt=8" target="_blank">iOS</a> and <a href="https://play.google.com/store/apps/details?id=com.vitruviussoftware.bunifish.asteroidtracker&feature" target="_blank">Android</a> as well as related apps. 

 Get <a href="http://apps.getpebble.com/en_US/application/55bc4913d1690c372900000f" target="_blank">Asteroid Today on Pebble</a> 

Follow us on <a href="https://twitter.com/AsteroidTracker" target="_blank">Twitter</a>

## Authorization

This API does not require authorization.

## Actions

### Find Near Earth Objects by date

> Get a list of Near Earth Objects within a date range, The max range in one query is 7 days

*Tags:* `feed`

#### Input Parameters
* `start_date` - _optional_ - Start of date range search, format: yyyy-MM-dd - (ex: 2015-04-28)
* `end_date` - _required_ - End of date range search, format: yyyy-MM-dd - (ex: 2015-04-28). If left off search will extends 7 days from start_date
* `detailed` - _optional_ - detailed

### Find Near Earth Objects for today

> Get a list of Near Earth Objects for today

*Tags:* `feed`

#### Input Parameters
* `detailed` - _optional_ - detailed

### Browse the Near Earth Objects service

> Retieve a paginated list of Near Earth Objects

*Tags:* `neo`

#### Input Parameters
* `page` - _optional_ - page
* `size` - _optional_ - size

### Retrieve Sentry (Impact Risk ) Near Earth Objects

> Retrieves Near Earth Objects listed in the NASA sentry data set

*Tags:* `neosentry`

#### Input Parameters
* `is_active` - _optional_ - show current list of Sentry objects, or show removed Sentry objects
* `page` - _optional_ - page
* `size` - _optional_ - size

### Retrieve Sentry (Impact Risk ) Near Earth Objectby ID

> Retrieves Sentry Near Earth Object by ID

*Tags:* `neosentry`

#### Input Parameters
* `asteroid_id` - _required_ - ID of NearEarth object.  ID can be SPK_ID, Asteroid des (designation) or Sentry ID

### Find Near Earth Objects by id

> Retrieve a Near Earth Objects with a given id

*Tags:* `neo`

#### Input Parameters
* `asteroid_id` - _required_ - ID of Near Earth Object - (ex: 3729835)

### Get the Near Earth Object data set totals

> retrieveCurrentNeoStatistics

*Tags:* `stats`

## License

**flow**ground :- Telekom iPaaS / neowsapp-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
