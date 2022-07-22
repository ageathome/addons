# &#127960; Age@Home
The [Age@Home](http://github.com/ageathome) add-on has the following configuration parameters:

+ `mqtt` - \ MQTT broker
+ `oveview` - overview image or service
+ `w3w` - [What3Words](http://what3words.com) location
+ `uptimerobot_rssurl` - [UptimeRobot](http://uptimerobot.com) RSS feed

# Configuration

## `mqtt`
A MQTT broker is required for this add-on; the MQTT add-on (_core-mosquitto_) is recommended.

```
host: core-mosquitto
port: 1883
username: username
password: password
```

## `overview`
The overview image displayed may be configured for the following modes:

+ `local` - use the local `image` specified
+ `hybrid` - use Google Maps; requires `apikey`

A Google developer account is required to generate an API key.

```
apikey: <Google Maps API key>
image: overview.jpg
mode: local
zoom: 18
```

### [What3Words](http://what3words.com)
The location of devices and other entities may be specified using this service; a free developer account is required to generate an API key.

 + `words` - location as `///your.three.words`
 + `apikey` - API key for access to service

```
apikey: <API key>
words: ///your.three.words
```


### [UptimeRobot](http://uptimerobot.com)

+ `uptimerobot_rssurl` - RSS URL feed

```
http://rss.uptimerobot.com/<Unique identifier>
```

# `MQTT`
A `MQTT` broker is required; the default [`mosquitto`](https://github.com/home-assistant/hassio-addons/tree/master/mosquitto) add-on is sufficient, but must be configured with appropriate authentication, for example:

```
- username: username
  password: password
```

