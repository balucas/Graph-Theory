## Theorems/Definitions

**Characteristic Vector**: Let $G$ be a graph and $S$ be a spanning subgraph of $G$. The characteristic vector $w_s$ of $S$ is::the $\{0,1\}$ vector with coordinates indexed by the edge set of $G$ where the $e^{th}$ coordinate is $1$ if $e \in E(G)$ and $0$ otherwise.

**Flow Space**::The flow space of a graph $G$ is the set of all characteristic vectors $w_s$ of even spanning subgraphs $S$ of $G$.

**Addition in the Flow Space**: For even subgraphs $S$ and $T$ of $G$, $S \oplus T$ =::the set of vectors $w_{s \oplus t} = w_s \oplus w_t$ 

**Theorem**: Let $G$ be a graph and let $H$ be an even spanning subgraph of $G$.::There exists cycles $C_1, ..., C_k$ in $G$ such that $E(H) = \cup_{i=1}^k E(C_i)$ and $E(C_i) \cap E(C_j) = \emptyset$ for all $i \neq j$.

**Fundamental Cycle**: Let $G$ be a connected graph and let $T$ be a spanning tree of $G$.::For any edge $e \in E(G) \backslash E(T)$, the graph $T + e$ has $1$ cycle $C_e$ , called the fundamental cycle for $e$ w.r.t. $T$.

**Theorem**: Let $G$ be a connected and $T$ be a spanning tree of $G$. Then a basis of $W(G)$ is::$B_T = \{w_C : C \in F(T)\}$ where $F(T)$ denotes the set of fundamental cycles w.r.t $T$ and $w_C$ is the characteristic vector of the even spanning subgraph of $G$ with edge set $E(C)$.

**Corollary**: If $G$ is connected, then $W(G)$ has dimension::$|E(G)|-|V(G)|+1$.

**Size of $W(G)$**: Let $n=|V(G)|$ and $m=|E(G)|$, then::$|W(G)| = 2^{m-n+1}$

**Binary Codes**::A binary code of length $m$ is a subspace $U$ of $\mathbb{Z}_{2}^{m}$. 

**Minimum Distance**::The minimum distance of $U$ is the smallest $t$ such that there exists $u \neq 0$ in $U$ with exactly $t$ $1$-coordinates.

**Hamming Distance**::The Hamming distance between $u \in U$ and $v \in U$ is the number of $1$-coordinates in $u\oplus v$.

**Lemma**: Let $U$ be a binary code with minimum distance $t$. Then::any 2 distinct elements of $U$ are at Hamming distance at least $t$.

**Girth**::The length of the shortest cycle in $G$. ($\infty$ if $G$ is a forest)

**Lemma**: Let $G$ be a graph with finite girth $g$. $W(G)$ is::a binary code of length $m=|E(G)|$, dimension $m-n+1$ where $n=|V(G)|$, and minimum distance $g$.

**Smallest # of Vertices in a Graph Given Min. Degree $\delta$ and Girth $g$**::$n_o(\delta, g) = \{1+\frac{\delta}{\delta-2}((\delta-1)^{\frac{g-1}{2}}-1)\}$ if $g$ is odd and $\{\frac{2}{\delta-2}((\delta-1)^{\frac{g}{2}}-1)\}$ if $g$ is even.

**Lemma**: Any graph $G$ with girth $g$ and minimum degree $\delta$ has::at least $n_o(\delta, g)$ vertices.

**Moore Graph**::The graph with minimum degree $\delta$ and girth $g$ and exactly $n_o(\delta, g)$ vertices.

**Lemma**: Let $G$ be a connected $\delta$-regular graph and let $A$ be the adjacency matrix of $G$. Then::the unit vector is an eigenvector of $A$ with multiplicity 1.