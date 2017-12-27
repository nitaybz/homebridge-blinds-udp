# homebridge-blinds-udp
Control your Blinds through UDP packets

*inspired by Homebridge-NooLite-HTTP-Blinds by JenRus

_________________________________________
#### Creating and maintaining Homebridge plugins consume a lot of time and effort, if you would like to share your appreciation, feel free to "Star" or donate. 

<a target="blank" href="https://www.paypal.me/nitaybz"><img src="https://img.shields.io/badge/Donate-PayPal-blue.svg"/></a>
<a target="blank" href="https://blockchain.info/payment_request?address=18uuUZ5GaMFoRH5TrQFJATQgqrpXCtqZRQ"><img src="https://img.shields.io/badge/Donate-Bitcoin-green.svg"/></a>

[Click here](https://github.com/nitaybz?utf8=%E2%9C%93&tab=repositories&q=homebridge) to review more of my plugins.
_________________________________________

# config.json

```
{
        "accessory": "BlindsUDP",
        "name": "My Blinds",
        "host": "192.168.0.X",
        "port": 80,
        "up_payload": "874652395hjui4d98523",
        "down_payload": "8932y4123545j5k245325",
        "stop_payload": "43523632641512",
        "motion_time": "5000"
}
```

## Configuration Params

|             Parameter            |                       Description                       | Required |
| -------------------------------- | ------------------------------------------------------- |:--------:|
| `name`                           | name of the accessory                                   |     ✓    |
| `host`                           | endpoint for whatever is receiving these requests       |     ✓    |
| `port`                           | port of destination                                     |     ✓    |
| `up_payload`                     | payload for the up state (open)                         |     ✓    |
| `down_payload`                   | payload for the down state  (close)                     |     ✓    |
| `stop_payload`                   | payload for the stop state                              |     ✓    |
| `motion_time`                    | time which your blind needs to move from up to down (ms)|     ✓    |

## Help

  - Make sure to specify a port and host in the config file.

## Installation

1. Install homebridge using: `npm install -g homebridge`
2. Install this plugin using: `npm install -g homebridge-blinds-udp`
3. Update your config file
