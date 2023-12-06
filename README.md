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
Because we know that our two graphs of interest have the same number of nodes we know it is at least possible for a function between them to be one-to-one and onto. Because both graphs are fully connected, we also know that each node in $G_1$ is equivalent to each other other node in $G_1$ in how many edges they both have, we also know this for $G_2$. We also know that each node in $G_1$ is equivalent to each node in $G_2$ at least with respect to how many edges there are attached to each of them. If we map a vertex in $G_1$ to a vertex in $G_2$ every edge connected to our vertex in $G_1$ will map to an edge connected to our mapped vertex in $G_2$. This means that any mapping with no repetition from each node in $G_1$ to $G_2$ will be one-to-one and onto. A particular function that can map from one graph to the other can be constructed by taking all of the nodes from $G_1$ taking a random permutation of those nodes, then taking all of the nodes from $G_2$, and taking a random permutation of those nodes. Then for each node in our permutation of $G_1$ we map that node to a node in our permutation of $G_2$ with no repetition. This will create a one-to-one and onto mapping from $G_1$ to $G_2$ and thus, they are isomorphic.
