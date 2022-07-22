# &#127960; Age@Home
The [Age@Home](http://github.com/ageathome) add-on has the following configuration parameters:

+ `mqtt` - MQTT broker
+ `oveview` - Overview image
+ `w3w` - [What3Words](http://what3words.com) location
+ `uptimerobot_rssurl` - [UptimeRobot](http://uptimerobot.com) RSS feed

# Configuration

## MQTT

A `MQTT` broker is required; the default [`mosquitto`](https://github.com/home-assistant/hassio-addons/tree/master/mosquitto) add-on is sufficient, but must be configured with appropriate authentication, for example:

## `mqtt`
```
- username: username
  password: password
```

### MQTT integration

A MQTT broker is required for this add-on; the MQTT add-on (_core-mosquitto_) is recommended.

```
host: core-mosquitto
port: 1883
username: username
password: password
```

## `overview`
The overview image displayed may be configured for the following modes:

+ `local` - use the local _image_ specified
+ `hybrid` - use Google Maps; requires _apikey_

A Google developer account is required to generate an API key.

```
apikey: <Google Maps API key>
image: overview.jpg
mode: local
zoom: 18
```

### [`w3w`](http://what3words.com)
The location of devices and other entities may be specified using this service; a free developer account is required to generate an API key.

 + `words` - location as `///your.three.words`
 + `apikey` - API key for access to service

```
apikey: <API key>
words: ///your.three.words
```


### [`uptimerobot_rssurl`](http://uptimerobot.com)

A RSS URL that provides updates from the service; the _unique identifier_ requires a free account.

```
http://rss.uptimerobot.com/<Unique identifier>
```
