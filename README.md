# Isomorphism

Prove that if two graphs $A$ and $B$ have the same number of nodes and are
completely connected, they must be isomorphic. I have started with the formal
definition of isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

## My Response, Maxie M. 

### Understanding of the Problem

**Let grpahs be denoted as:**
- $A = (V_1 , E_1)$
- $B = (V_2 , E_2)$

  **where:**
  - $V_1$ and $V_2$ will be the vertex sets of $A$ and $B$, respectively
  - $E_1$ and $E_2$ will be the edge sets of $A$ and $B$, respectively

  **Given Information:**
  - The graph will have the same number in vertices, so $|V_1| = |V_2|$
  - $E_1$ and $E_2$ are complete graphs with all possible edges
    - Due to every pair of distinct vertices in each graph will be connected by an edge

### Definition of Graph Isomorphism 
- Two graphs are said to be **isomorphc** if a bijection exists such that for all vertices $u, v \in V_1$
  - Graph One: $G_1 = (V_1, E_1)$
  - Graph Two: $G_2 = (V_2, E_2)$
  - Bijection: one-to-one and onto function $f: V_1 \to V_2$
-  We have: $(u, v) \in E_1 \iff (f(u), f(v)) \in E_2$
  - There is a one-to-one correspondence between the verties of $A$ and $B$
    - two vertices $u$ and $v$ in $A$ are connected if and only if their corresponding vertices $f(u)$ and $f(v)$ in $B$ are connected

### Bijection for Completely Connected Graphs 
- **Since graphs $A$ and $B$ are both connected:**
  - Every pair of distinct vertices is connected by an edge
    - meaning, edge set $E_1$ of graph $A$ will contain all pairs of distinct vertices from $V_1$
    - and, edge set $E_2$ of graph $B$ will contain all pairs of distinct vertices from $V_2$
- **Establishing a cBijection That Perserves Adjacency Between Vertices**
  - **one-to-one and onto:** can be established by matching each vertex in $V_1$ to exactly one vertex in $V_2$ and **vice versa*
    - Due to $|V_1| = |V_2| and both grpahs having the same number of vertices 
  - **Adjacency Preservation:** In a complete graph, every pair of distinct vertices is connected by an egde
    - Due to $A$ and $B$ both being complete graphs, mapping $f$ will map each vertex in $V_1$ to a unique vertex in $V_2$
    - every pair of distinct vertices in $A$ will correspond to a pair of distinct vertices in $B$
    - for every pair of vertices $u, v \in V_1$ we have $(u,v) \in E_1$ and $(f(u), f(v)) \in E_2$
      - This ensures the preservation of adjacency

### Conlusion 
- Due to being able to establish a bilection that perverses the edge structure (adjacency) of the graphs
- Concluding that the two completely connected graphs $A$ and $B$ are **isomorphic*

### Plagiarism Statement:
I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.

### Resources:
- https://networkx.org/nx-guides/content/algorithms/isomorphism/isomorphism.html
