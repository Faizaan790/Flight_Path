# Flight_Path

## Overview

This project involves the implementation and testing of a weighted graph using Java. The main goal is to complete the `WeightedGraph` class and test it using the `UseGraph.java` driver.

## How to Run the Project

1. Clone the repository to your local machine:
   ```sh
   git clone https://github.com/yourusername/weighted-graph-project.git
   
2. Navigate to the project directory:
   ```sh
   cd weighted-graph-project
3. Add the following lines of code to the UseGraph.java driver to test the hasVertex method:
   ```sh
   System.out.println("The graph has Atlanta: " + graph.hasVertex(s0));
   System.out.println("The graph has L.A.: " + graph.hasVertex("L.A."));
   
- To compile and run the UseGraph.java driver:
```sh
  javac UseGraph.java
  java UseGraph
 ```
## Example Output:
<pre>
The graph has Atlanta: true
The graph has L.A.: false
Determining path using depth first ...
Austin to Chicago
Austin
Houston
Atlanta
Washington
Dallas
Denver
Chicago
true
...
Shortest paths starting at Washington
Last Vertex Destination Distance
------------------------------------
Washington Washington 0
Washington Atlanta 600
Atlanta Houston 1400
The unreachable vertices are:
Austin
Chicago
Dallas
Denver
...
</pre>

