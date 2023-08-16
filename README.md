## Quadrifilar Helix Antenna for 868 MHz
Quadrifilar Helix Antenna is hemi-spherical circularly polarized antenna. It's ability to directionally receive or transmit of circularly polarized radiation while minimizing unwanted radiation perfect fits especially for satellite communication. This 3D model helps to achieve correct shape of antenna segments which has crucial effect for correct circular polarization and antenna tunnig.

![light 3D printable QFH antenna design](pictures/QFH-Antenna.png)

Antenna is made from 2 pcs of 0.8mm silver plated copper wire, with total length 357 mm and 339.4 mm.
<img src="pictures/QFH-Antenna-868MHz.jpg" width="400" />

# Antenna feed-point

The connection point to the antenna is created by the [antenna balun](https://github.com/ODZ-UJF-AV-CR/QFHBAL01). That solution allows easy use of an RG174 coaxial cable with MCX or optionally SMA connector.

# Antenna Frequency characteristic

<img src="pictures/QFH-Antenna-868MHz-S11.png" />
<img src="pictures/QFH-Antenna-868MHz-SmithChart.png" />
<img src="pictures/QFH-Antenna-868MHz-VSWR.png" />

Calculated in:
http://jcoppens.com/ant/qfh/calc.en.php

<b>Warning. 3D model add parasitic capacity to antenna which moves resonant frequency. This was corrected by calculating antenna for higher frequeny (913 MHz). Changing any parameter must be verified by measurement.</b>

![Calculated parameters](https://github.com/cernohorsky/QFH-Antenna-868MHz/blob/master/pictures/QFH-Antenna-868MHz-Param.jpg)
For explanation of the prameters refer to [this page](https://uuki.kapsi.fi/qha_simul.html).

