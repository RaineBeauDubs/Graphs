# Graph Notes:
  - Graphs are a way to quantify data.
    # Directed Graph:
      - restricted traversal
      - (can be?) cyclic 
      - "one-way directions"
      - ex:
        ~ singly-linked list
        ~ following celebrities on twitter
    # Undirected Graph:
      - can traverse either way
      - "no directions or multiple directions"
      - ex:
        ~ doubly-linked list
        ~ facebook friend relationships
  - Density is measured by number of *edges,* not the number of nodes.
  - Ways to kep track of info in graphs:
    # adjacency list:
      - dictionaty with nodes as keys and lists of nodes as values
      - complexity: O(n^2)
      - actually pretty good for dense graphs
    # matrix
    # object-oriented approach

  - We assume that a list of edges is unordered when we are doing a depth-first- or bredth-first-traversal.
  - Difference between search and traversal:
    - search stops once you find the thing you're looking for
    - traversals touch every single node

  # Bredth-First-Traversals:
    - Okay, it's better now, but hard to write in words.
    - Psudocode Steps:
      - create a queue
      - create list of visited nodes
      - put starting node in queue
      # while (queue not empty):
        - pop node out of queue
        # if not visited:
          - mark as visited
          - get adjacent edges and add to queue
    
  # Depth-First-Traversals:
  - uses a stack instead of a queue, of course
  - Psudocode Steps:
    - create a stack
    - create list of visited nodes
    - put starting node in stack
    # while (stack not empty):
      - pop top node out of stack
      # if not visited:
        - mark as visited
        - get adjacent edges and add to stack


# Definitions:
  # arc:
    directed line (a pair of ordered vertices)
  # edge:
    line joining a pair of nodes
      ~ incident edges: edges that share a vertex, "A[n] edge and vertex are incident if the edge connects the vertex to another."
  # loop:
    edge or arc that joins a vertex to itself
  # vetex (node):
    a point (or circle), fundamental unit that make graphs
      ~ adjacent vertacies: connected by edge
      ~ degree: number of edges connected to said vertex (loops count twice)
      ~ predecessor/successor
  # weight:
    values/numbers assigned(?) to edges