## Theorems/Definitions

**Matching**:
?
A matching $M$ in a graph $G$ is a set of disjoint edges (i.e. no vertex of $G$ is incident to more than one edge of $M$).

A matching $M$ {{saturates}} a vertex $v$ if $v$ is incident to an edge of $M$. Otherwise, $v$ is {{$M$-exposed}}.

**Maximum Matching**::A matching in $G$ of maximum possible size.

**Perfect Matching**::A matching in $G$ that saturates $V(G)$ 

Greedy Matching Algorithm
?
(Graph $G$) -> Matching $M$
1. Set $M:= \emptyset$ and $H:=G$ 
2. If $H$ has no edges, return $M$ 
3. Else: Choose $xy\in E(H)$. Set $M:= M\cup \{xy \}$. Set $H:= H-\{xy\}$.
4. Go to 2

Greedy Matching Algorithm Pros/Cons
?
Pro: Easy to implement and efficient
Con: Doesn't always give a maximum matching

**Matching Number**::The max size of a matching in $G$, written $\nu (G)$ 

**Theorem**: The greedy algorithm always finds {{a matching of size $\geq \frac{\nu(G)}{2}$}} in $G$. 

**Hall's Theorem**:
?
Let $G$ be a bipartite graph with vertex classes $X$ and $Y$. Then, G has a matching saturating $X$ if and only if for every $S\subseteq X$, $|N(S)| \geq |S|$ 

**Corollary**: Any bipartite graph that is {{$r$-regular, with $r\geq 1$}}  has a {{perfect matching}}.

**Hall's Theorem (Defect Ver.)**
?
Let $d\geq 0$, and let $G$ be a bipartite graph with vertex classes $X$ and $Y$. Then $G$ has a matching of size $|X|-d$ if and only if $|N(S)| \geq |S| - d$ for  each $S\subseteq X$. 

**Vertex Cover**
?
A vertex cover (of the edges) in graph $G$ is a set $W\subseteq V(G)$ such that every edge of $G$ is incident to some vertex of $W$. (i.e. $G-W$ has no edges).
The minimum size of a vertex cover in $G$ is denoted $\tau (G)$ 

**Konig's Theorem**
?
If $G$ is bipartite, then $\tau(G) = \nu(G)$.

**Edge Cover**
?
An edge cover (of vertices) of a graph $G$ is a set of edges $F$ of $G$ such that each $v\in V(G)$ is incident to an edge of $F$.
The minimum size of an edge cover of $G$ is denoted $\rho(G)$

**Lemma**: For any $G$, $\alpha(G) + \tau(G)$ {{$=|V(G)|$}}

**Gallai's Theorem**: 
?
For every $G$ with no isolated vertices, $\nu(G) + \rho(G) = |V(G)|$
