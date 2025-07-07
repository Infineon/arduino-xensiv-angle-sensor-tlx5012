# XENSIV™ TLx5012B Angle Sensor

[![.github/workflows/compile_examples.yml](https://github.com/Infineon/arduino-xensiv-angle-sensor-tlx5012/actions/workflows/compile_examples.yml/badge.svg?branch=devops%2Frelease-lib-wflow-enable)](https://github.com/Infineon/arduino-xensiv-angle-sensor-tlx5012/actions/workflows/compile_examples.yml)

Arduino library of Infineon's highly sensitive [XENSIV™ TLx5012B](https://www.infineon.com/cms/en/product/sensor/magnetic-sensors/magnetic-position-sensors/angle-sensors) 360° magnetic angle sensor.

### Suported Products

| <img src="https://raw.githubusercontent.com/Infineon/xensiv-angle-sensor-tlx5012/main/docs/img/TLE_5012B_DSO-8-16_plain.png" width=150 style="background:white"> | <img src="https://raw.githubusercontent.com/Infineon/xensiv-angle-sensor-tlx5012/main/docs/img/TLE5012B_breakout.png" width=150 style="background:white"> | <img src="https://raw.githubusercontent.com/Infineon/xensiv-angle-sensor-tlx5012/main/docs/img/TLE5012B_horizontal.png" width=400 style="background:white"> |
|:--:|:--:|:--:|
| *bulk sensor* | *breakout board* | *Sensor2Go kit* 


This library supports also all predefined communication variants IIF, PWM, SPC. All of these variants also support the SSC interface.

### Supported Frameworks

The library supports all Infineon XMC microcontroller and Arduino and Arduino compatible devices which can handle a 3Wire (SSC) SPI interface. Therefore have a look at the list of [compatible and tested kits](href="https://xensiv-angle-sensor-tlx5012.readthedocs.io/en/latest/) as well as at the [Porting Guide](href="https://xensiv-angle-sensor-tlx5012.readthedocs.io/en/latest/). You are maybe able to get it running with the right SPI pin setting and a sufficient resistor setup.


## Summary
The [XENSIV™ TLx5012B](https://www.infineon.com/cms/en/product/evaluation-boards/tle5012b_e1000_ms2go/) is a 360° angle sensor that detects the orientation of a magnetic field. This is achieved by measuring sine and cosine angle components with monolithic integrated Giant Magneto Resistance (iGMR) elements. These raw signals (sine and cosine) are digitally processed internally to calculate the angle orientation of the magnetic field (magnet). The XENSIV™ TLx5012B is a pre-calibrated sensor. The calibration parameters are stored in laser fuses. At start-up the values of the fuses are written into flip-flops, where these values can be changed by the application-specific parameters. Further precision of the angle measurement over a wide temperature range and a long lifetime can be improved by enabling an optional internal auto calibration algorithm. Data communications are accomplished with a bi-directional Synchronous Serial Communication (SSC) that is SPI-compatible. The sensor configuration is stored in registers, which are accessible by the SSC interface. Additionally four other interfaces are available with the XENSIV™ TLx5012B: Pulse-Width-Modulation (PWM) Protocol, Short-PWM-Code (SPC) Protocol, Hall Switch Mode (HSM) and Incremental Interface (IIF). These interfaces can be used in parallel with SSC or alone. Pre-configured sensor derivate with different interface settings are available.

## Key Features and Benefits
* Giant Magneto Resistance (GMR)-based principle
* Integrated magnetic field sensing for angle measurement
* 360° angle measurement with revolution counter and angle speed measurement
* Two separate highly accurate single bit SD-ADC
* 15 bit representation of absolute angle value on the output (resolution of 0.01°)
* 16 bit representation of sine / cosine values on the interface
* Max. 1.0° angle error over lifetime and temperature-range with activated auto-calibration
* Bi-directional SSC Interface up to 8 Mbit/s
* Interfaces: SSC, PWM, Incremental Interface (IIF), Hall Switch Mode (HSM), Short PWM Code (SPC, based on SENT protocol defined in SAE J2716)
* Output pins can be configured (programmed or pre-configured) as push-pull or open-drain
* Bus mode operation of multiple sensors on one line is possible with SSC or SPC interface


## Contributing
This is a release repository for the Arduino framework. The code base is maintained and developed in the High-Side-Switch Cross-Framework-Platform (XFP) library [repository](https://xensiv-angle-sensor-tlx5012.readthedocs.io/en/latest/index.html).

## Documentation
The complete documentation of the library as well as detailed information about the XENSIV™ TLx5012B Angle Sensor, can be found [here](https://xensiv-angle-sensor-tlx5012.readthedocs.io/en/latest/index.html).


## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
