---
layout: page
title: "IMAP Sensor"
description: "Instructions how to integrate IMAP sensors into Home Assistant."
date: 2016-07-11 06:00
sidebar: true
comments: false
sharing: true
footer: true
ha_category: Sensor
ha_release: 0.25
---


The `imap` sensor platform is observing your [IMAP server](https://en.wikipedia.org/wiki/Internet_Message_Access_Protocol) and reporting the amount of unread emails.

To enable this sensor, add the following lines to your `configuration.yaml` file:

```yaml
# Example configuration.yaml entry
sensor:
  - platform: imap
    server: imap.gmail.com
    port: 993
    name: Emails
    user: USERNAME
    password: PASSWORD
```

Configuration variables:

- **server** (*Required*): The IP address or hostname of the IMAP server.
- **port** (*Required*): The port where the server is accessible.
- **name** (*Optional*): Name of the IMAP sensor.
- **user** (*Required*): Username for the IMAP server.
- **password** (*Required*): Password for the IMAP server.

