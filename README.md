
# METRO APP SYSTEM

**OVERVIEW**
Develop a comprehensive Metro App System aimed at optimizing the efficiency
of metro operations in a city, enhancing commuter experience, and facilitating
seamless metro network management. The system should address key
challenges in metro transportation, providing solutions for route planning,
station management, passenger information, and overall operational
optimization.

**TOPICS USED**
1. C++ Language and Object Oriented Programming:
      • Classes and Objects: The program utilizes classes like station and user to
      encapsulate station details and user information, respectively.
      • Encapsulation: Data members (like stations map, idpassword,
      metrocardbalance) and member functions (like fare(), display(),
      updatebalance()) are encapsulated within these classes to control access
      and maintain data integrity.
2. Set (Data Structure):
      • Employed within the adjacency list (adjList) to represent connections
      between stations.
3. Vector:
      • Used to store and manage paths between source and destination
      stations (allPaths).
4. Map:
      • It's used to store station information, mapping station IDs to station
      names (metroSystem.stations)..
5. Graph Data Structure:
        • Adjacency List Representation:
        The program uses an adjacency list to represent the metro system. The
        adjlist variable is an unordered map where each key represents a station,
        and the corresponding value is a set of pairs containing adjacent stations
        and their respective distances.• Path Finding – Depth First Search:
        - The DFS algorithm is used to find all possible paths between a given
        source and destination station.
        - Within the findAllPaths() function, DFS is implemented using a stack to
        traverse through the graph, exploring all possible paths until the
        destination station is reached.
        -The algorithm maintains a stack of visited nodes and backtracks
        whenever it encounters a dead end until all possible paths are explored.
6. Dijkstra's Algorithm:
        - The program also calculates the shortest distance between stations using
        Dijkstra's algorithm.
        - The shortestdistance() function utilizes a set to manage distances and
        applies a variation of Dijkstra's algorithm to find the shortest path from the
        source station to all other stations in the graph.
7. File Handling:
      - Employs file handling to store and retrieve user counts and user details in
      external files (‘usercount.txt’) and (‘userdetails.txt’).
