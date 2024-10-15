# Dijkstra's Shortest Path Algorithm

## Overview
This project implements the Dijkstra algorithm for finding the shortest paths in a weighted graph. The graph is represented as an adjacency list, and a priority queue is used to efficiently find the minimum path. The solution is written in Java.

## Features
- Add vertices and edges dynamically to the graph.
- Compute the shortest path from a starting vertex to all other vertices.
- Handles graphs with positive edge weights.

## How to Use

1. **Add Vertices**: You can add vertices using the `addVertex` method.
2. **Add Edges**: Connect the vertices using the `addEdge` method, specifying the source, destination, and weight.
3. **Run Dijkstra's Algorithm**: Call the `dijkstra(startVertex)` method to find the shortest paths from the specified vertex.

### Example

```java
Graph graph = new Graph();

graph.addVertex("A");
graph.addVertex("B");
graph.addVertex("C");
graph.addVertex("D");
graph.addVertex("E");

graph.addEdge("A", "B", 5);
graph.addEdge("A", "C", 1);
graph.addEdge("B", "D", 2);
graph.addEdge("C", "B", 2);
graph.addEdge("C", "D", 8);
graph.addEdge("D", "E", 6);
graph.addEdge("C", "E", 3);

System.out.println("Shortest paths from A: " + graph.dijkstra("A"));
