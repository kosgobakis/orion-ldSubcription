# Problem with subscriptionOrion-LD  v1.0.0

## Orion-LD 0.8.0
Set 0.8.0 in .env

Run test, notification send
```json
[
  {
    "id": "urn:ngsi-ld:Subscription:61e1c79e38075c532edeb815",
    "type": "Subscription",
    "description": "Notify me of all changes",
    "entities": [
      {
        "type": "TemperatureSensor"
      }
    ],
    "watchedAttributes": [
      "temperature"
    ],
    "notification": {
      "attributes": [
        "temperature"
      ],
      "format": "normalized",
      "endpoint": {
        "uri": "http://tonowhere",
        "accept": "application/json"
      },
      "timesSent": 1,
      "lastNotification": "2022-01-14T18:57:34.692Z"
    },
    "@context": "http://context/minimal.jsonld"
  }
]
```

## Orion-LD 1.0.0 
Set 1.0.0 in .env

Run test, no subscription send
```json
[
  {
    "id": "urn:ngsi-ld:Subscription:61e1c7ecc13481d816421313",
    "type": "Subscription",
    "description": "Notify me of all changes",
    "entities": [
      {
        "type": "TemperatureSensor"
      }
    ],
    "watchedAttributes": [
      "temperature"
    ],
    "notification": {
      "attributes": [
        "temperature"
      ],
      "format": "normalized",
      "endpoint": {
        "uri": "http://tonowhere",
        "accept": "application/json"
      }
    },
    "@context": "http://context/minimal.jsonld"
  }
]
```