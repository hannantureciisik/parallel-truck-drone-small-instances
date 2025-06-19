Small-sized Instances for "The Stochastic Location-Routing Problem with Parallel Truck-Drone Operations for Humanitarian Aid Delivery"

Note: No endurance limit is imposed for small-sized instances.
Each instance includes 15 demand nodes (indexed from 0), 5 candidate depot nodes, and 10 disaster scenarios.


Each instance folder contains the following files:

- complete.txt
  Binary adjacency matrix (n × n) showing road network connections between demand nodes and candidate depots (subset of demand nodes). A value of 1 indicates a direct road edge; 0 indicates no direct connection.

- t.txt
  Matrix of truck travel times between demand nodes and candidate depots. Only values corresponding to an edge in complete.txt should be used. Non-zero values where complete.txt has 0 indicate indirect routes and should be ignored.

- v.txt
  Matrix of drone return trip durations between all node pairs (i.e. round-trip drone travel times between any two nodes).

- W.txt
  Each line represents one candidate depot (i.e. one demand node ID per line).

- D_k.txt
  Each line corresponds to the depot on the same line in W.txt (e.g. the first line in D_k.txt is for the depot listed on the first line of W.txt, and so on). Each line lists demand nodes reachable by drone from that depot, separated by commas, sorted in non-decreasing order of drone return trip time from the demand node to the depot.
