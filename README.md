# PhoenixDrone
Open-Source Releases of our Phoenix Drone tail-sitter MAV. 

<img src="http://www.starslab.ca/wp-content/themes/stars-lab/images/stars-logo.png" width="500">

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
If you use any of these resources in your work, please cite the [relevant publication](https://arxiv.org/abs/1810.03196): 

```
@inproceedings{2019_Wu_Phoenix,
  address = {Montreal, Quebec, Canada},
  author = {Yilun Wu and Xintong Du and Rikky Duivenvoorden and Jonathan Kelly},
  booktitle = {Proceedings of the {IEEE} International Conference on Robotics and Automation {(ICRA})},
  doi = {10.1109/ICRA.2019.8794433},
  pages = {5330--5336},
  title = {The Phoenix Drone: An Open-Source Dual-Rotor Tail-Sitter Platform for Research and Education},
  url = {https://arxiv.org/abs/1810.03196},
  year = {2019},
}
```
