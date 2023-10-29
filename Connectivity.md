## Definitions / Theorems

**Component**::A maximal connected subgraph.

**Cut Vertex**::A vertex $x$ of a connected graph $G$ such that $G-x$ is disconnected.

**Vertex Cut**::A set of vertices $W$ in a connected graph $G$ such that $G-W$ is disconnected.

**K-Connected**: A graph $G$ is $k$-connected if {{$|V(G)| \geq k + 1$}} and {{$G$ has no vertex cut of size $\leq k - 1$}}.

If $G$ is $k$-connected, it is also {{$l$-connected for all $l \leq k$}}.

**Minimum Degree**::denoted by $\delta(G)$.

**Lemma**: {{Let $G$ be a $k$-connected graph where $k \geq 1$}}. {{Then $\delta(G) \geq k$}}.

**(Lemma) Minimum Degree Condition for Large Connectivity**: Let $G$ be a graph with $n$ vertices where $1\leq k \leq n-1$.
?
If $\delta(G) \geq \frac{n+k-2}{2}$, then $G$ is $k$-connected.

**Lemma**: If $G$ is $2$-connected and $xy, xz \in E(G)$ are distinct edges, then {{there exists a cycle in $G$ containing both $xy$ and $xz$}}.

**Lemma**: Let $e_1, e_2, e_3$ be edges such that $e_1$ and $e_2$ lie in a common cycle and $e_2$ and $e_3$ lie in a common cycle. Then, {{$e_1$ and $e_3$ lie in a common cycle}}.

**Characterization of $2$-Connected Graphs**: Let $G$ be a graph with $|V(G)|\geq 3$. The following are equivalent:
?
1. $G$ is $2$-connected.
2. $G$ has no isolated vertices.
3. Any 2 vertices lie in a common cycle.

**Contraction**: The graph $G/e$ obtained by contracting $e$ has vertex set {{$V(G) \backslash \{x,y\} \cup \{z\}$}} where $e=xy$ and $z$ is a new vertex.

**Lemma**: Let *G* be a *2*-connected graph and suppose $\{x,y\}$ is a $2$-vertex cut in $G$. Let $C_1$ be a component of $G-\{x,y\}$. Then graph $H$ with vertex set $V(C_1) \cup \{x,y\}$ and edge set $\{wz \in E(G): w,z \in V(H)\} \cup \{x,y\}$ is {{$2$-connected}}.

**Lemma**: Let $G_1$ and $G_2$ be {{$k$-connected graphs such that $|V(G_1) \cap V(G_2)| \geq k$}}, then {{graph $G$ with $V(G) = V(G_1) \cup V(G_2)$ and $E(G) = E(G_1) \cup E(G_2)$}} is {{$k$-connected}}.

**Corollary**: Let $G$ be a $2$-connected graph and $e \in E(G)$. If {{$|V(G) \geq 4|$}}, then either {{$G \backslash e$ is $2$-connected}} or {{$G / e$ is $2$-connected}}.

**Theorem**: Let $G$ be a $2$-connected graph. Then at least $1$ of the following holds: {{$G$ is a cycle}}, {{there exists an edge $e \in E(G)$ such that $G \backslash e$ is $2$-connected}}, or {{$G$ is the $2$-sum of a $2$-connected graph and a cycle}}.

How to construct any $2$-connected graph: start with {{a cycle}} and step by step either {{adding an edge between any $2$ vertices already present}} or {{subdividing an edge that is present}}.
