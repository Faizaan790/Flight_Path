<h1>How to run this project on your local machine</h1>
Test the completed implementation using the UseGraph.java file.
If you try to run the UseGraph driver without completing the implementation of the WeightedGraph
class, the output will not be correct.
When implementing hasVertex, use the equals method to compare vertices.

Add the following lines of code to test the hasVertex method:
System.out.println("The graph has Atlanta: " + graph.hasVertex(s0));
System.out.println("The graph has L.A.: " + graph.hasVertex("L.A."));
The correct output of the UseGraph driver should be the following:

**Creating graph in figure 10.3
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
Austin to Washington
Austin
Houston
Atlanta
Washington
true
Dallas to Austin
Dallas
Denver
Atlanta
Washington
Houston
Chicago
Austin
true
Atlanta to Denver
Atlanta
Washington
Dallas
Denver
true
Washington to Dallas
Washington
Dallas
true
Washington to Austin
Washington
Dallas
Denver
Chicago
Austin
true
Determining path using breadth first ...
Austin to Chicago
Austin
Dallas
Houston
Chicago
true
Austin to Washington
Austin
Dallas
Houston
Chicago
Denver
Atlanta
Washington
true
Dallas to Austin
Dallas
Austin
true
Atlanta to Denver
Atlanta
Houston
Washington
Dallas
Austin
Chicago
Denver
true
Washington to Dallas
Washington
Atlanta
Dallas
true
Washington to Austin
Washington
Atlanta
Dallas
Houston
Austin
true
Shortest paths starting at Washington
Last Vertex Destination Distance
------------------------------------
Washington Washington 0
Washington Atlanta 600
Washington Dallas 1300
Atlanta Houston 1400
Dallas Austin 1500
Dallas Denver 2080
Dallas Chicago 2200
The unreachable vertices are:
Shortest paths starting at Denver
Last Vertex Destination Distance
------------------------------------
Denver Denver 0
Denver Chicago 1000
Denver Atlanta 1400
Atlanta Washington 2000
Atlanta Houston 2200
Washington Dallas 3300
Dallas Austin 3500
The unreachable vertices are:
Creating graph in figure 10.x
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
Austin to Washington
Austin
Houston
Atlanta
Washington
true
Washington to Houston
Washington
Atlanta
Houston
true
Washington to Dallas
Washington
Atlanta
Houston
false
Washington to Austin
Washington
Atlanta
Houston
false
Determining path using breadth first ...
Austin to Chicago
Austin
Dallas
Houston
Chicago
true
Austin to Washington
Austin
Dallas
Houston
Chicago
Denver
Atlanta
Washington
true
Washington to Houston
Washington
Atlanta
Houston
true
Washington to Dallas
Washington
Atlanta
Houston
false
Washington to Austin
Washington
Atlanta
Houston
false**
**Shortest paths starting at Washington
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
Shortest paths starting at Denver
Last Vertex Destination Distance
------------------------------------
**Denver Denver 0
Denver Chicago 1000
Denver Atlanta 1400
Atlanta Washington 2000
Atlanta Houston 2200**
**The unreachable vertices are:
Austin
Dallas ****
