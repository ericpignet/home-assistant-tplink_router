# TPLink Router device tracker for Home Assistant
[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg)](https://hacs.xyz/)

The `tplink_router` platform for `device_tracker` integration allows you to detect presence by looking at connection devices to a [TP-Link](https://www.tp-link.com) wireless router.

It was part of the official `tplink` integration in the past but was [removed](https://github.com/home-assistant/core/pull/27936) from Home Assistant.

## Installation
Recommended: use [HACS](https://hacs.xyz/).

Manual: copy `custom_components/tplink_router` folder into your `custom_components`.

## Configuration
```yaml
# Example configuration.yaml entry
device_tracker:
  - platform: tplink_router
    host: YOUR_ROUTER_IP
    username: YOUR_ADMIN_USERNAME
    password: !secret tplink_router_password
```

## Supported devices
- Archer C7 firmware version 150427
- Archer C9 firmware version 150811
- EAP-225 AP with latest firmware version
- Archer D9 firmware version 0.9.1 0.1 v0041.0 Build 160224 Rel.59129n
- TPLink N600 with latest firmware
- VR600 with latest firmware
- TL-WR840N 
- TL-WDR4900

If your device is not in the list, you can still give it a try and let me know if it works or not, I'll update the documentation.

*Disclaimer*: I cannot add support for devices I don't own, but external contributions are definitely welcome. Feel free to open an issue on Github if you want to help.

## Documentation
See [README](https://github.com/ericpignet/home-assistant-tplink_router/blob/master/README.md) for full documentation.
