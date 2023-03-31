# Graphs

## To turn in your reading “Reply” to this discussion by teaching something that you learned.

- Graph - A graph is a collection of nodes/vertices that can be connected to each other by line segments called edges.
  - Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
  - Edge - An edge is a connection between two nodes.
  - Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
  - Degree - The degree of a vertex is the number of edges connected to that vertex.
- Undirected Graphs - An Undirected Graph is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.
  - ![Undirected-Graphs](401-Notes/assets/Undirected.png)
- Directed Graphs (Digraph) - A Directed Graph also called a Digraph is a graph where every edge is directed.

  - ![Directed-Graph](401-Notes/assets/DIrected.png)

Unlike an undirected graph, a Digraph has direction. Each node is directed at another node with a specific requirement of what node should be referenced next.

- Complete Graphs - A complete graph is when all nodes are connected to all other nodes.

  - ![Complete-Graphs](401-Notes/assets/Complete.png)

- Connected - A connected graph is graph that has all of vertices/nodes have at least one edge.

  - ![Connected](401-Notes/assets/Connected.png)

- Disconnected - A disconnected graph is a graph where some vertices may not have edges.

  - ![Disconnected](401-Notes/assets/Disconnected.png)

- Acyclic Graph - An acyclic graph is a directed graph without cycles. A cycle is when a node can be traversed through and potentially end up back at itself.

  - ![Acyclic-Graph](401-Notes/assets/Acyclic.png)

- Cyclic Graphs - A Cyclic graph is a graph that has cycles. A cycle is defined as a path of a positive length that starts and ends at the same vertex.

  - ![Cyclic-Graphs](401-Notes/assets/Cyclic.png)

- Adjacency Matrix - An Adjacency matrix is represented through a 2-dimensional array. If there are n vertices, then we are looking at an n x n Boolean matrix. Each Row and column represents each vertex of the data structure. The elements of both the column and the row must add up to 1 if there is an edge that connects the two, or zero if there isn’t a connection.
  - We follow this same pattern for the other vertex’s and where they are connected.
  - We follow this same pattern for the other vertex’s and where they are connected.
  - If there is not an edge/connection between the vertex’s, we represent this by placing a 0 in the appropriate point of the matrix.

    - ![Adjacency-Matrix](401-Notes/assets/Adjancency Matrix.png)

  - a sparse graph is when there are very few connections. a dense graph is when there are many connections

- Adjacency List - An adjacency list is the most common way to represent graphs. An adjacency list is a collection of linked lists or array that lists all of the other vertices that are connected. Adjacency lists make it easy to view if one vertices connects to another.
  - Looking at the original graph that we are representing, we can see that Vertex A has an edge to both Vertex C and Vertex D. As a result, we will place both Vertex C and Vertex D in the adjacency list. Just from observation, we can see that we will only place the vertices that are connected in the list. If there is no connection between the vertices, they are not listed.
  - Thinking about how we will implement this in code? Well, let’s look at what the visual is telling us.
    - We can visually see that we are working with a collection of some sort. The visual is depicting a Linked List, but you could easily make it an array of arrays if you’d like.
    - Each index or node (depending on the data structure you choose to represent the adjacency list) will be a vertex within the graph.
    - Every time you add an edge, you will find the appropriate vertices in the data structure and add it to the appropriate location.

  - ![Adjacency-List](401-Notes/assets/Adjacency List.png)

- Weighted Graphs - A weighted graph is a graph with numbers assigned to its edges. These numbers are called weights. This is what a weighted graph looks like:

When representing a weighted graph in a matrix, you set the element in the 2D array to represent the actual weight between the two paths. If there is not a connection between the two vertices, you can put a 0, although it is known for some people to put the infinity sign instead.

- ![Weighted-Graphs](401-Notes/assets/Weighted Graphs.png)

  - Using the graph from above, here is an example of what a weight matrix would look like:

  Within adjacency lists, you must include both the weight and the name of the adjacent vertex.

  - ![Weighted-List](401-Notes/assets/Weighted List.png)

- Traversals - You will be required to traverse through a graph. The traversals itself are like those of trees. Below is a breakdown of how you would traverse a graph.
  - Breadth First - In a breadth first traversal, you are starting at a specific vertex/node. This node must be specified when calling the BreadthFirst() method. The breadth first traversal of a graph is like that of a tree, with the exception that graphs can have cycles. Traversing a graph that has cycles will result in an infinite loop….this is bad. To prevent such behavior, we need to have some way to keep track of whether a vertex has been “visited” before. Upon each visit, we’ll add the previously-unvisited vertex to a visited set, so we know not to visit it again as traversal continues.

  - ![Breadth-First](401-Notes/assets/Traversal BreadthFirst.png)

  - As a refresher of what breadth first actually means here it is: Breadth first traversal is when you visit all the nodes that are closest to the root as possible. From there you traverse outwards, level by level, until you have visited all the vertices/nodes.
    - Enqueue the declared start node into the Queue.
    - Create a loop that will run while the node still has nodes present.
    - Dequeue the first node from the queue
    - if the Dequeue‘d node has unvisited child nodes, add the unvisited children to visited set and insert them into the queue.

  - Depth Firt - In a depth first traversal, our approach is a bit different than the approach used for breadth first. While the breadth first traversal uses a Queue to visit all children at a given level, the depth first traversal uses a Stack to visit all children of a given subtree. (This differs from our approach to tree traversal, where we visit nodes via recursive calls. Recursive calls use a call stack internally.)
  
  - ![Depth-Firt](401-Notes/assets/Traversal Depth First.png)

  - Push the root node into the Stack and mark as visited.
  - Start a while loop that runs as long as the stack is not empty.
  - Pop the top node off of the stack and check its neighbors.
  - If a neighbor hasn’t been visited, push it onto the stack and mark as visited
  - Repeat until the stack is empty.

[link-to-reding-notes](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/graphs.html).


************************************************************************************ 

### Things I want to know more about:

How will we be using this in class?