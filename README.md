# PhoenixDrone
Open-Source Releases of the PhoenixDrone Tail-sitter Project


## License
The PhoenixDrone is released under the MIT license.

Copyright (c) <2018> [STARS Lab](http://www.starslab.ca/)

<img src="http://www.starslab.ca/wp-content/themes/stars-lab/images/stars-logo.png" width="500">

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.


## Mechanical Components
An overall mechanical CAD design document, 3D-print-ready model files, and a BOM (Bill of Materials) required to assemble PhoenixDrone is provided under `PhoenixDrone-MCAD`. For details, refer to the README of the submodule repo.

## SITL Simulation
A set of Gazebo Plug-ins required for PhoenixDrone SITL simulation is provided under `PhoenixDrone-sitl_gazebo`. This submodule contains a gazebo model description file for the complete PhoenixDrone model as well as a calibrated aerodynamic model for the vehicle.

## MATLAB Simulink Model
A high-fidelity MATLAB simulink model is released for easy, quick and accurate simulation of the dynamics and motion control of PhoenixDrone. The models can be found under `PhoenixDrone-Simulink`.

## BLHeli ESC Firmware
Our modified BLHeli firmware released under `BLHeli` allows DYS-SN20A ESCs to send synchronous pulses at phase commutations to the flight computer which processes the timestamps of these signals to infer motor speeds. Please refer to the README of the repo for compiling and flashing ESC firmware. 

## PX4 Flight Code
The `PX4-PhoenixDrone` repo contains all of the flight code (controller, state estimator, state machine, drivers, communication software) running onboard the flight computer. One may use QGroundControl (the default PX4 GCS), or any MAVlink-enabled clients such as MAVROS to communicate with the onboard computer to receive telemetry and send commands.

## Contact
Please e-mail Yilun Wu at <yl.wu@robotics.utias.utoronto.ca> for any questions regarding the resources and its usage released here.
  
## Citation
If you use any of these resources in academic work, please cite the [relevant publication](https://arxiv.org/abs/1810.03196): 

```bibtex
@conference{PhoenixDrone,
	Author = {Yilun Wu and Xintong Du and Rikky Duivenvoorden and Jonathan Kelly},
  Title = {The Phoenix Drone: An Open-Source Dual-Rotor Tail-Sitter Platform for Research and Education},
	Booktitle = {Proceedings of IEEE International Conference on Robotics and Automation (ICRA'19)},
	Note = {To Appear},
	Year = {2019}}
```
