# Scotland Yard data
The data is usable for a Scotland Yard map with stations from 1 to 199. There is an other version that ends at 200 but the station 108 is missing in this version.

The base version of the data was created by @frog32, but I, @AlexElvers, have corrected many station positions and connections.

## stations.txt
The station number, x-position, y-position and the station type are separated by a space.
```
1 190 40 taxi,bus,underground
2 487 20 taxi
3 675 25 taxi,bus
4 790 15 taxi
...
```

## connections.txt
Both stations and the connection type are separated by a space. The first station is smaller than the second as there are no one-ways and the data is an undirected graph. Whenever there is a connection from A to B, you have to ensure that it is possible to move from B to A.
```
108 115 water
115 157 water
157 194 water
1 46 underground
13 46 underground
...
```
