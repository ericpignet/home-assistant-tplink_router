# TPLink Router device tracker for Home Assistant

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

## Documentation
See [README](https://github.com/ericpignet/home-assistant-tplink_router/blob/master/README.md) for full documentation.