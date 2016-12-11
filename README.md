# powerdatamining
This repository is destinated to pull information about how to extract metadata from the openstreetmap api.
# Downloading the data...
I found this way for extract information into the openstreetmap data base with the power #tag, the file bolivia_power.osm is converted to bolivia_power.csv, the useful information into this .csv file is just nodes,ways,relations ids and some metadata related with ids, for extract the position (lat,lon,relations,tags)related with this ids create this litle programs.
The file extract_data_1.1.py outs 6x .npy  files. For example for the node 12345634 into the bolivian_power.csv the related metadata into the openstreetmap api http://api.openstreetmap.org/api/0.6/node/12345634/  is in a <xml> format wich is pull it into the position [0] of the  nodes.npy file and so on  to complete all the ids, whem the ids change to "ways" tag, the code pulls the contend of http://api.openstreetmap.org/api/0.6/way/... into the way.npy file with his respective information.

# Cleaning the data ...
