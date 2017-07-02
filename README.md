# Extended Kalman Filter
This Project is the sixth task (Project 1 of Term 2) of the Udacity Self-Driving Car Nanodegree program. The main goal of the project is to apply Extended Kalman Filter to fuse data from LIDAR and Radar sensors of a self driving car using C++.

The project was created with the Udacity [Starter Code](https://github.com/udacity/CarND-Extended-Kalman-Filter-Project).

## Content of this repo
- `scr` a directory with the project code:
  - `main.cpp` - reads in data, calls a function to run the Kalman filter, calls a function to calculate RMSE
  - `FusionEKF.cpp` - initializes the filter, calls the predict function, calls the update function
  - `kalman_filter.cpp`- defines the predict function, the update function for lidar, and the update function for radar
  - `tools.cpp` - a function to calculate RMSE and the Jacobian matrix
- `data`  a directory with two input files, provided by Udacity
- `results`  a directory with output and log files
- `Docs` a directory with files formats description


## How to run the code
Clone this repo and perform 
```
mkdir build && cd build
cmake .. && make
./ExtendedKF ../data/obj_pose-laser-radar-synthetic-input.txt output1.txt > input1.log
```

The resulted output files are supplied in the [results](results) directory.


