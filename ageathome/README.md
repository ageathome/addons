# &#127960; Age@Home

The [Age@Home](http://age-at-home.com) ([github](http://github.com/ageathome)) _add-on_ 
for [Home Assistant](http://home-assistant.io) provides a **replacement** configuration 
that processes multiple classes of sensor data (e.g. _motion_) using the extensive portfolio of 
Home Assistant [integrations](https://www.home-assistant.io/integrations), including [Shelly](http://shelly.cloud)
and many other vendors.

## Status

![](https://img.shields.io/github/license/ageathome/core.svg?style=flat)
![](https://img.shields.io/github/release/ageathome/core.svg?style=flat)
[![Build Status](https://travis-ci.org/dcmartin/ageathome.svg?branch=master)](https://travis-ci.org/dcmartin/ageathome)
[![Coverage Status](https://coveralls.io/repos/github/ageathome/core/badge.svg?branch=master)](https://coveralls.io/github/dcmartin/open-horizon?branch=master)

![](https://img.shields.io/github/repo-size/ageathome/core.svg?style=flat)
![](https://img.shields.io/github/last-commit/ageathome/core.svg?style=flat)
![](https://img.shields.io/github/commit-activity/w/ageathome/core.svg?style=flat)
![](https://img.shields.io/github/contributors/ageathome/core.svg?style=flat)
![](https://img.shields.io/github/issues/ageathome/core.svg?style=flat)
![](https://img.shields.io/github/tag/ageathome/core.svg?style=flat)

## Containers

![](https://img.shields.io/badge/amd64-yes-green.svg)[![](https://images.microbadger.com/badges/image/dcmartin/amd64-addon-ageathome.svg)](https://microbadger.com/images/dcmartin/amd64-addon-ageathome)[![](https://images.microbadger.com/badges/version/dcmartin/amd64-addon-ageathome.svg)](https://microbadger.com/images/dcmartin/amd64-addon-ageathome)[![](https://img.shields.io/docker/pulls/dcmartin/amd64-addon-ageathome.svg)](https://hub.docker.com/r/dcmartin/amd64-addon-ageathome)
![](https://img.shields.io/badge/aarch64-yes-green.svg)[![](https://images.microbadger.com/badges/image/dcmartin/aarch64-addon-ageathome.svg)](https://microbadger.com/images/dcmartin/aarch64-addon-ageathome)[![](https://images.microbadger.com/badges/version/dcmartin/aarch64-addon-ageathome.svg)](https://microbadger.com/images/dcmartin/aarch64-addon-ageathome)[![](https://img.shields.io/docker/pulls/dcmartin/aarch64-addon-ageathome.svg)](https://hub.docker.com/r/dcmartin/aarch64-addon-ageathome)
![](https://img.shields.io/badge/armv7-yes-green.svg)[![](https://images.microbadger.com/badges/image/dcmartin/armv7-addon-ageathome.svg)](https://microbadger.com/images/dcmartin/armv7-addon-ageathome)[![](https://images.microbadger.com/badges/version/dcmartin/armv7-addon-ageathome.svg)](https://microbadger.com/images/dcmartin/armv7-addon-ageathome)[![](https://img.shields.io/docker/pulls/dcmartin/armv7-addon-ageathome.svg)](https://hub.docker.com/r/dcmartin/armv7-addon-ageathome)

<hr>

# &#9995; MQTT required

A MQTT broker is required; the default
[_core-mosquitto_](https://github.com/home-assistant/hassio-addons/tree/master/mosquitto)
add-on is recommended; it must be configured with appropriate authentication, for example:

## `Logins`

```
- username: username
  password: password
```

<hr>

## Changelog & Releases
Releases are based on Semantic Versioning, and use the format
of ``MAJOR.MINOR.PATCH``. In a nutshell, the version will be incremented
based on the following:

- ``MAJOR``: Incompatible or major changes.
- ``MINOR``: Backwards-compatible new features and enhancements.
- ``PATCH``: Backwards-compatible bugfixes and package updates.

## Authors & contributors
David C Martin (github@dcmartin.com)
