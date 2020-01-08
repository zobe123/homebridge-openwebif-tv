# homebridge-openwebif-tv
[![npm](https://img.shields.io/npm/dt/homebridge-openwebif-tv.svg)](https://www.npmjs.com/package/homebridge-openwebif-tv) [![npm](https://img.shields.io/npm/v/homebridge-openwebif-tv.svg)](https://www.npmjs.com/package/homebridge-openwebif-tv)

Control plugin for Sat Receivers basis on the OpenWebIf interface (Dreambix, VU+, etc..).
Present in HomeKit as TV service, schange channels, volume/mute control, power control.

This plugin is basis on homebridge-openwebif-switch created by alex224.

HomeBridge: https://github.com/nfarina/homebridge

# Installation

1. Install homebridge using: npm install -g homebridge
2. Install homebridge-openwebif-tv using: npm install -g homebridge-openwebif-tv
3. Update your configuration file. See sample-config.json in this repository for a sample. 

# Limitations
Due to HomeKit app limitation max. channels in bouquets is 98. Over this value HomeKit app will no response.

# Info 

# Configuration

 <pre>
"accessories": [
        {
            "accessory": "OpenWebIfTv",
            "name": "Tuner Sat",
            "host": "192.168.1.10",
            "port": 80,
            "speakerService": true,
            "bouquets": [
            {
              "name": "Das Erste HD",
              "reference": "1:0:19:283D:3FB:1:C00000:0:0:0:"
            },
            {
              "name": "ZDF HD",
              "reference": "1:0:19:2B66:3F3:1:C00000:0:0:0:"
            },
            {
              "name": "RTL HD",
              "reference": "1:0:19:EF10:421:1:C00000:0:0:0:"
            },
            {
              "name": "SAT.1 HD",
              "reference": "1:0:19:EF74:3F9:1:C00000:0:0:0:"
            },
            {
              "name": "ProSieben HD",
              "reference": "1:0:19:EF75:3F9:1:C00000:0:0:0:"
            },
            {
              "name": "RTLII HD",
              "reference": "1:0:19:EF15:421:1:C00000:0:0:0:"
            }
       ]
     }
    ]
</pre>


# Whats new:
https://github.com/grzegorz914/homebridge-openwebif-tv/blob/master/CHANGELOG.md

# Development
- Pull request and help in development highly appreciated.
