# CircularFlightPattern
An implementation of a circular flight pattern for use by a 3D multimedia display, a Dronevision (DV).  We provide two algorithms for an FLS to travel from its current coordinate to rendezvous with its assigned slot on the flight pattern, Shortest Distance (SD) and Fastest Rendezvous Time (FRT).

Authors:  Shuqin Zhu (shuqinzh@usc.edu) and Shahram Ghandeharizadeh (shahram@usc.edu)

## A Demonstration
Click the image below to watch the YouTube clip of the implementation using 5 Crazyflies with the Vicon localization technique.

[![A Demonstration](https://github.com/flyinglightspeck/CircularFlightPattern/blob/main/simulation.png)](https://www.youtube.com/watch?v=_hcwj3lhY5g)


## Clone
``git clone https://github.com/flyinglightspeck/CircularFlightPattern.git``

## Requirements
Python 3.9 with
numpy,
matplotlib,
pandas,
scipy.

## Instructions to Run
Install Python 3.9 with the required libraries.  

To run the simulator, execute the script implement_simu.py, i.e., issue the command `python implement_simu.py` or `python3 implement_simu.py`.  If using Mac OS, uncomment the line `mpl.use('macosx')` in implement_simu.py.

The simulator runs either the Shortest Distance (SD) or the Fastest Rendezvous Time (FRT) algorithm.  Adjust the value `path_policy` in config.py to run FRT (`path_policy=0`) or SD (`path_policy=1`).  

To require the simulator to visualize its execution, set `fresh_rate=1` in config.py.

## Acknowledgments
This research was supported in part by the NSF grants IIS-2232382 and CMMI-2425754.
