# Jarvis-iot

[![License Apache 2][badge-license]](LICENSE)
[![GitHub version](https://badge.fury.io/gh/zeiot%2Frasphome.svg)](https://badge.fury.io/gh/zeiot%2Frasphome)

* Master : [![Circle CI](https://circleci.com/gh/zeiot/jarvis/tree/master.svg?style=svg)](https://circleci.com/gh/zeiot/jarvis/tree/master)
* Develop: [![Circle CI](https://circleci.com/gh/zeiot/jarvis/tree/develop.svg?style=svg)](https://circleci.com/gh/zeiot/jarvis/tree/develop)

Features :

* [ ] Analyze the indoor / outdoor temperature ([DHT22][])
* [ ] Measure air quality ([MQ135][])

Requirements:

* [RaspberryPI][]
* [Arduino][]

## Arduino

* For *arduino* projects, we use [PlatformIO][], initialize it:

        $ make arduino-init

* For project (here *dht*) setup arduino devices client configurations:

        $ cp arduino/dht/src/config.sample.h arduino/dht/src/config.h
        # edit config.h to customize your requirements

* Build project (for example dht):

        $ make arduino-build project=arduino/dht

* Connect an Arduino, then upload it :

        $ make arduino-upload project=arduino/dht


## Development

See [DEV](DEV.md)


## Contributing

See [CONTRIBUTING](CONTRIBUTING.md).


## License

See [LICENSE](LICENSE) for the complete license.


## Changelog

A [changelog](ChangeLog.md) is available


## Contact

Nicolas Lamirault <nicolas.lamirault@gmail.com>




[badge-license]: https://img.shields.io/badge/license-Apache2-green.svg?style=flat

[RaspberryPI]: https://www.raspberrypi.org/
[PlatformIO]: http://platformio.org/
[Arduino]: https://www.arduino.cc/

[DHT22]: https://www.adafruit.com/products/385
[MQ135]: https://www.olimex.com/Products/Components/Sensors/SNS-MQ135/
