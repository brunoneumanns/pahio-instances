# PaHIO-instances

This repository contains instances of the parcel delivery problem with heterogeneous locker boxes and inbound and outbound demand (PaHIO).

In the folder named `bs`, you find instances based on the city of Braunschweig, Germany. In that folder, you find four subfolders with data describing each instance.

* `capacities`: data indicating the number of locker boxes by size and by station.
* `commodities`: data describing the parcels as inbound and outbound demand.
* `coordinates`: data indicating the location of each depot and each station.
* `distances`: data describing origin-destination distances.

In order to run an experiment, you need to select a file from each of these folders, according to the following convention:

* The integer number next to the letter `d` shows how many depots there are in the instance.
* The integer number next to the letter `s` shows how many stations there are in the instance.
* The substring `bs` indicates that the instance is based on the city of Braunschweig.

In the folder `commodities`, we also consider the following convention:

* q[high|mid|low]: intensity of inbound demand.
* o[high|mid|low]: intensity of outbound demand.
* The integer number next to the letter `t` shows how many time periods there are in the instance (from 0 to that integer number).

Example:

An instance may consist of the following files:

* d2_s5_bs_capacities.csv
* d2_s5_bs_coordinates.csv
* d2_s5_bs_distances.csv
* d2_s5_bs_qhigh_o_mid_t11_commodities.csv

If you want to run an experiment on the same physical infrastructure with different demand, you can select a different commodity file, as this coincides with the number of depots and stations.
