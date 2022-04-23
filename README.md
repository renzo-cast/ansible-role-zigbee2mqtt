# Zigbee2MQTT Ansible Role

The unofficial ansible role for installing and configuring [Zigbee2MQTT](https://www.zigbee2mqtt.io).

Instructions from <https://www.zigbee2mqtt.io/guide/installation>

**This role is currently only compatible with Debian installs and has only been tested on a Raspberry Pi (Buster)**

## Requirements

N/A

## Role Variables

For more details on these configuration variables see <https:#github.com/mikebrady/shairport-sync/blob/development/scripts/shairport-sync.conf>

| Variable Name | Default |
| -- | -- |
| mqtt_base_topic | `zigbee2mqtt` |
| mqtt_server | `localhost` |
| mqtt_port | `1883` |s
| zigbee2mqtt_version | `HEAD` |
| zigbee2mqtt_network_key | `GENERATE` |
| zigbee2mqtt_user | `pi` |
| device_brand | `` |

## Dependencies

### collections

* community.general

## Example Playbook

```yaml
roles:
    - role: ansible-role-zigbee2mqtt
```

## License

MIT
