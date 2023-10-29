## Definitions / Theorems

**Block**::A non-empty connected graph with no cut vertex ($2$-connected).

A {{block of a group $G$}} is {{a subgroup of $G$ that is maximal with respective to being a block}}.

**Block-Cut Vertex Forest of Connected G**::A bipartite graph with vertex classes $B$ and $C$ where $B$ is the set of blocks of $G$ and $C$ is the set of cut vertices of $G$.

**Edge Set of Block-Cut Vertex Forest**::$\{bc : b\in B, c\in C, bc \in E(G)\}$.

**Theorem**: The block-cut vertex forest of a connected graph is {{a tree}}.

**End-Block**::A block with degree $1$ in the BCF of $G$ is the end-block of $G$ that's connected but not $2$-connected.

All {{vertices of degree 1}} in a BCF of $G$ are blocks since {{every cut-vertex is in $\geq 2$ blocks of $G$}}.

**Theorem K1**:{{Let $G$ be a connected graph such that every block of $G$ is planar}}. {{Then $G$ is planar}}.