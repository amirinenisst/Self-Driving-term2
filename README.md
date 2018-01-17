# Unscented kalman filter
The main objective of this project is to estimate the state of a moving object of interest with noisy lidar and radar measurements by using unscented Kalman filter.
This projects fuses both the values from Lidar and Radar.

## Building
The main program can be built and run by doing the following from the project top directory.
mkdir build
cd build
cmake ..
make
./ExtendedKF

## Code 

src- a directory with the project code:
main.cpp - reads in data, calls a function to run the Kalman filter, calls a function to calculate RMSE
ukf.cpp - the UKF filter itself, defines the predict function, the update function 
tools.cpp - a function to calculate RMSE
data a directory with input file
results a directory with output file

## Results: <a name="results"></a>

- position accuracy
![](images/img.JPG) 
- position accuracy
![](images/img1.JPG) 

## Other Important Dependencies
* cmake >= 3.5
  * All OSes: [click here for installation instructions](https://cmake.org/install/)
* make >= 4.1 (Linux, Mac), 3.81 (Windows)
  * Linux: make is installed by default on most Linux distros
  * Mac: [install Xcode command line tools to get make](https://developer.apple.com/xcode/features/)
  * Windows: [Click here for installation instructions](http://gnuwin32.sourceforge.net/packages/make.htm)
* gcc/g++ >= 5.4
  * Linux: gcc / g++ is installed by default on most Linux distros
  * Mac: same deal as make - [install Xcode command line tools](https://developer.apple.com/xcode/features/)
  * Windows: recommend using [MinGW](http://www.mingw.org/)



