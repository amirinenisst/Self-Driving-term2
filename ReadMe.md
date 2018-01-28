# Kidnapped vehicle project

The main objective of this project is helping to localize a car in an unknown location.

## Building
The main program can be built and run by doing the following from the project top directory.
```
mkdir build
cd build
cmake ..
make
./particle_filter
```

## Inputs to the Particle Filter
We can find the inputs to the particle filter in the data directory.

### The Map*
map_data.txt includes the position of landmarks (in meters) on an arbitrary Cartesian coordinate system. Each row has three columns
```
x position
y position
landmark id
```
### Control Data
control_data.txt contains control data. Each row corresponds to the control data for the corresponding time step. Columns represent 
vehicle speed (in meters per second)
vehicle yaw rate (in radians per second)

### Observation Data
The observation directory contains files that are numbered corresponding to the timestep with respect to observation.


