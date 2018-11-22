# Traveling Salesman Problem

Based on https://developers.google.com/optimization/routing/tsp and https://en.wikipedia.org/wiki/Travelling_salesman_problem

---

The Traveling Salesman Problem (TSP) is one of the most famous problems in computer science. In what follows, we'll describe the problem and show you how to find a solution.

+++

The travelling salesman problem (TSP) asks the following question: "Given a list of cities and the distances between each pair of cities, what is the shortest possible route that visits each city and returns to the origin city?" It is an NP-hard problem in combinatorial optimization, important in operations research and theoretical computer science.

---

# The problem

Back in the days when salesmen traveled door-to-door hawking vacuums and encyclopedias, they had to plan their routes, from house to house or city to city. The shorter the route, the better. Finding the shortest route that visits a set of locations is an exponentially difficult problem: finding the shortest path for 20 cities is much more than twice as hard as 10 cities.

+++

An exhaustive search of all possible paths would be guaranteed to find the shortest, but is computationally intractable for all but small sets of locations. For larger problems, optimization techniques are needed to intelligently search the solution space and find near-optimal solutions.

+++

Mathematically, traveling salesman problems can be represented as a graph, where the locations are the nodes and the edges (or arcs) represent direct routes between the nodes. The weight of each edge is the distance between the nodes. The goal is to find the path with the shortest sum of weights. Below, we see a simple four-node graph and the shortest cycle that visits every node: 

+++

In addition to finding solutions to the classical Traveling Salesman Problem, OR-Tools also provides methods for more general types of TSPs, including the following:

+++

Asymmetric cost problems—The traditional TSP is symmetric: the distance from point A to point B equals the distance from point B to point A. However, the cost of shipping items from point A to point B might not equal the cost of shipping them from point B to point A. OR-Tools can also handle problems that have asymmetric costs.
Prize-collecting TSPs, where benefits accrue from visiting nodes
TSP with time windows

---

