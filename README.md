# ETTRPTWData
This repository provides the dataset used in the Electric Truck and Trailer Routing Problem with Time Windows (ETTRPTW).

The instances are formatted as follows:

###For each location the instance provides:
-StringId as a unique identifier
-Type indicates the function of the location, i.e,
---d: depot
---f: recharging station
---c1:  truck customer location
---c2:  vehicle customer location
-x, y are coordinates (distances are assumed to be euclidean) 
-demand specifies the quantity of freight capacity required
-ReadyTime and DueDate are the beginning and the end of the time window (waiting is allowed)
-ServiceTime denotes the entire time spend at customer for loading operations

###For the electric vehicles (all identical):
-"E Vehicle fuel tank capacity": units of energy available
-"W^1 Truck load capacity":      units available for cargo
-"W^2 Trailer load capacity":      units available for cargo
-"F^1 Truck cost":      acquisition cost of a solo truck unit
-"F^2 Complete vehicle cost":      acquisition cost of a truck carrying a trailer unit
-"alpha Energy consumption per unit distance":      reduction of battery capacity when traveling one unit of distance
-"beta Energy replenished per unit waiting time":     units of time required to recharge one unit of energy
-"v average Velocity":           assumed to be constant on all arcs, required to calculate the travel time from distance

Modifications required for adapting this dataset to the EVRPTW and ESDVRPTW variants are discussed in Section 5 of the paper.
Feel free to email me if you have any questions: ahbassaleh@shockers.wichita.edu
