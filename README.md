![logo pyAutonomousAgent_small](https://github.com/user-attachments/assets/91ee7bac-81f0-4994-a557-8a672d9ca124)

## pyAutonomousAgent

pyAutonomousAgent is an open-source academic tool for modeling autonomous agent behaviors through behavior trees.
The tool is an open-source set of computer routines, which was developed with the aim of being easy to use and learn.
A detailed explanation of this tool can be found in [Medeiros 2024].

In this tool the behavior trees are implemented through the python library py-trees [py-trees 2020]. 

As a study case, the tool provides two simulation scenarios with swarms of autonomous agents.
There are two types of autonomous agents:
- a simplified computational model of a drone with a two-dimensional motion model; and
- a computational model of the Skywalker X8 drone.

PyFly-fixed-wing tool [Bohn et al. 2019] was used to simulate the Skywalker X8 drone inside the pyAutonomousAgent tool. 
PyFly-fixed-wing tool provides computational implementation of a 6 Degrees Of Freedom (DOF) aerodynamic model of the Skywalker X8 drone and its respective Proportional-Integral-Derivative (PID) controllers.
This aerodynamic model of the Skywalker X8 was proposed and validated in [Gryte et al. 2018].

The scenario with the swarm of drones is available in the file pyAutonomousAgents.ipynb. The scenario with the swarm of Skywalker X8 drones is available in the file pyAutonomousAgents_SkywalkerX8.ipynb.

The tool generates a graphical interface, which is an animated gif, based on the final result of the simulation.
The graphical interface is created through the python library celluloid [celluloi 2018].
An example of this interface can be seen in the file pyAutonomousAgent_simulation.gif.
The time interval to generate the gif file is proportional to the number of simulation frames recorded in this gif file. 
Therefore, this time interval can be reduced by decreasing the number of frames to be recorded, that is, increasing the variable step in the graphical part.

## Bibliographic References

Medeiros FLL (2024) pyAutonomousAgent: An Academic Tool for Modeling Autonomous Agent Behaviors Using Behavior Trees. In: Journal of Aerospace Technology and Management (JATM), vol. 16.

py-trees. c2020. Boston (MA): Daniel Stonier; accessed January 17, 2025. https://py-trees.readthedocs.io/en/devel/

Bohn E, Coates EM, Moe S, Johansen TA (2019) Deep reinforcement learning attitude control of fixed-wing UAVs using proximal policy optimization. Paper presented at: ICUAS 2019. Proceedings of the 2019 International Conference on Unmanned Aircraft Systems, USA.

Gryte K, Hann R, Alam M, Rohác J, Johansen TA, Fossen TI (2018) Aerodynamic modeling of the Skywalker X8 fixed-wing unmanned aerial vehicle. Paper presented at: ICUAS 2018. Proceedings of the 2018 International Conference on Unmanned Aircraft Systems, USA.

Celluloid 0.2.0. c2018. San Francisco Bay Area (CA): Jacques Kvam; accessed January 17, 2025. https://pypi.org/project/celluloid/
