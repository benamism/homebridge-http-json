# homebridge-http-json-sensors

This homebridge extension was designed to help me investigate how homebridge and homekit work together. To date, it should work with temperature, humidity and light levels, reported by an HTTP service as below.

Please feel free to update / extend!

# Forked from

This has been forked from lucacri/homebridge-http-temperature-humidity - thank you for all this excellent work!

# Installation (to be completed)

1. Install homebridge using: npm install -g homebridge
2. Install this plugin using: npm install -g homebridge-http-json-sensors
3. Update your configuration file. See sample-config.json in this repository for a sample. 

# Configuration


Configuration sample file:

 ```
"accessories": [
        "accessories": [
        {
            "accessory": "HttpJsonSensors",
            "name": "Living Room",
            "url": "http://192.168.1.210/sensors.json",
            "sendimmediately": "",
            "http_method": "GET"
        }
    ]

```


The JSON file should look something like this:
```
{
	"temperature": 25.8,
	"humidity": 38,
	"light-level": 300
}
