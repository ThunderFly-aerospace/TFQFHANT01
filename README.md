# TFQFHANT01 - Lightweight 3D-Printed Quadrifilar Helix Antenna for Telemetry

The **TFQFHANT01** module is a lightweight, 3D-printable Quadrifilar Helix (QFH) antenna designed for telemetry transmission from unmanned platforms, such as high-altitude stratospheric balloons. This design leverages a hemispherical, circularly polarized radiation pattern ideal for consistent communication with ground stations, particularly during varying orientations and altitude shifts typical of balloon trajectories.

![Light 3D-printed QFH antenna design](pictures/QFH-Antenna.png)

## Design and Construction

The antenna structure is composed of two 0.8mm silver-plated copper wires with lengths of **357 mm** and **339.4 mm**, respectively. These wires form the QFH loops and are fixed within a 3D-printed PLA framework to maintain accurate geometry, which is crucial for proper circular polarization and tuning. The antenna loops connect to the **QFHBAL01** balun module via soldered joints, ensuring a stable feed point with minimal signal loss.

The 3D-printed model is parametrically designed in [OpenSCAD](https://openscad.org/), allowing for easy adjustments to the antenna's dimensions and shape to meet specific frequency band and application requirements.

### Key Components

- **Antenna Material**: 0.8 mm silver-plated copper wire
- **Total Length of Helices**: 357 mm and 339.4 mm
- **3D-Printed Framework**: PLA material for lightweight and rigid support
- **Antenna Balun**: [QFHBAL01 PCB](https://github.com/mlab-modules/QFHBAL01) for balanced feed and improved impedance matching
- **Connector Compatibility**: RG174 coaxial cable with MCX or SMA connectors

## Frequency Tuning

This antenna is designed to operate at **868 MHz** but requires adjustment to compensate for parasitic capacitance introduced by the 3D model. The antenna was optimized by calculating its parameters for a higher target frequency (913 MHz) to achieve resonance at 868 MHz. Any modifications to antenna dimensions or materials should be re-validated through measurement to ensure proper tuning.

![Frequency response](pictures/QFH-Antenna-868MHz-S11.png)
![Smith Chart](pictures/QFH-Antenna-868MHz-SmithChart.png)
![VSWR](pictures/QFH-Antenna-868MHz-VSWR.png)

Calculations were conducted using [JCoppens’ QFH Calculator](http://jcoppens.com/ant/qfh/calc.en.php).

## Applications

This lightweight QFH antenna is optimized for high-altitude telemetry in stratospheric balloon applications, providing robust, circularly polarized transmission that is resilient to changes in the balloon’s orientation. Its circular polarization helps maintain reliable communication with ground-based receivers across a wide field of view, which is critical during balloon ascent, drift, and descent phases.

## Assembly Notes

- **Antenna Feed Point**: The QFHBAL01 balun offers a stable feed point with balanced impedance, supporting easy integration with coaxial cables. For optimum performance, verify feed-point alignment and secure all soldered connections.
- **Frequency Response Adjustment**: The inherent capacitance of the 3D-printed structure may affect resonance. Fine-tuning adjustments may be necessary if deviations from the calculated dimensions occur.

### Safety and Usage Notice

Adjustments to any parameters, including wire lengths or balun connection configurations, should be verified through measurements to maintain the intended performance characteristics. 

For detailed explanations of the QFH parameters and additional information, refer to [this resource](https://uuki.kapsi.fi/qha_simul.html).

