# **Extended Kalman Filter Project** 


---

**Extended Kalman Filter Project**

* Utilize a kalman filter to estimate the state of a moving object of interest with noisy lidar and radar measurements. 
* RMSE values that are lower than the tolerance outlined in the project 


---
### How to run the codes

This repository includes two files that can be used to set up and install uWebSocketIO for either Linux or Mac systems. For windows you can use either Docker, VMware, or even Windows 10 Bash on Ubuntu to install uWebSocketIO. 

Once the install for uWebSocketIO is complete, the main program can be built and run by doing the following from the project top directory.

- mkdir build
- cd build
- cmake ..
- make
- ./ExtendedKF

### Conclusion

Using lider and rader, I implemented codes using C++ to be able to check the distance and velocity of x and y between object and my car. Lider usually calculates distance between the object and my car. Rader takes responsibility for getting an information of velocity. Hence, in this project, those two sensors are fused to get those properties such as velocity and distance. Following charts show the results using RMSE which is mean squared error(MSE).

*Test One*

| Input |   MSE   |
| ----- | ------- |
|  PX   | 0.0973  |
|  PY   | 0.0855  |
|  VX   | 0.4513  |
|  VY   | 0.4399  |

*Test Two*

| Input |   MSE   |
| ----- | ------- |
|  PX   | 0.0977  |
|  PY   | 0.0859  |
|  VX   | 0.4516  |
|  VY   | 0.4399  |

