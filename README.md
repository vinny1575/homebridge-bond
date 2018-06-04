# homebridge-bond

Forked from edc1591.

I'll be adding more functions as time permits.

For now you can control the fan speed and lights (on/off no dimming yet)

# Installation
1. Install homebridge using `npm install -g homebridge`.
2. Install this plugin using `npm install -g git+https://github.com/vinny1575/homebridge-bond.git`.
3. Update your configuration file. See configuration sample below.

# Removal
1. Stop homebridge.
2. Remove configuration in `config.json`.
3. Start homebridge (the plugin will remove cached accessories automatically).
4. Remove this plugin using `npm remove -g homebridge-bond`.
5. Restart homebridge.

# Configuration
Edit your `config.json` accordingly. Configuration sample:
 ```
"platforms": [
    {
      "platform": "Bond",
      "email": "<email>",
      "password": "<password>"
    }
  ]
```
## Known Issues

The api doesn't retreive the device name for some reason. This plugin is using the device room and the type (Ex. Master Bedroom Fan, Master Bedroom Light). You can edit the names inside the Home application on your iOS device.

## Meta

Distributed under the MIT license. See ``LICENSE`` for more information.

[license-image]: https://img.shields.io/badge/License-MIT-blue.svg
[license-url]: LICENSE
