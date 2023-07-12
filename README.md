# snmp_integration
 Custom Homeassistant SNMP Integration

Heavily based on the official SNMP integration, found [here](https://www.home-assistant.io/integrations/snmp/). It holds all the same options and documentation as the original, but adds support for unique_id creation on switches, as well as adding typing and discovery_info support to be more in line with homeassistant integration standards.

The only notable change in usage is that the integration is held under `snmp_custom` instead of `snmp` in order to not confuse home assistant on config.

## Installation
### HACS Method
Install the HACS add-on through the HASS add-on store.

In the Integrations tab, press the 3 dots, and Custom repositories.

Paste this into the link: `https://github.com/blaketenantwatson/snmp_integration`, and select intergration, and then add.

You can now click on ssh integration in the Integrations tab, and then click download. Everything should now be setup.

### Manual Method
To get started clone this repository into `/config/`, so that the files are stored at:
```
/config/custom_components/ssh/__init__.py
/config/custom_components/ssh/switch.py
/config/custom_components/ssh/sensor.py
/config/custom_components/ssh/manifest.json
```

Restart, and the intergration should be setup. This method is less reliable than HACS, as HACS has some error checking for custom integrations that aren't done by HASS.
