[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=12685119&assignment_repo_type=AssignmentRepo)
# Isomorphism

Prove that if two graphs $A$ and $B$ have the same number of nodes and are
completely connected, they must be isomorphic. I have started with the formal
definition of isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

## Proof:

For a graph to be completely connected each vertex must have an edge that leads to every other vertex which means that every vertex in the graph must be equivalent to every other vertex, because every vertex has the same number of edges. Since we know that $A$ and $B$ have the same number of nodes and we know that each vertex within both of those graphs has the same number of edges, then any order of vertexes in $A$ can be mapped to any order of vertexes in $B$ and because these graphs are fully connected this will be a proper, isomorphic mapping.

## Better Proof(Maybe):
Because we know that our two graphs of interest have the same number of nodes we know it is at least possible for a function between them to be one-to-one and onto. Because both graphs are fully connected, we also know that each node in $G_1$ is equivalent to each other other node in $G_1$ in how many edges they both have, we know this for $G_2$. We also know that each node in $G_1$ is equivalent to each node in $G_2$ at least with respect to how many edges there are attached to each of them. This means that any mapping with no repetition from each node in $G_1$ to $G_2$ will be one-to-one and onto.
