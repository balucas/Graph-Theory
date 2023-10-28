## Theorems/Definitions

**Lemma**:  Let $G$ be a $k$-connected graph and let $Y\subset V(G)$ be a set of $k$ vertices in $G$. Then, the graph $H$ with {{$V(H) = V(G) \cup \{x \}$}} and edge set {{$E(G) \cup \{xy : y\in Y$}} is also $k$-connected.

**Fans**:
?
Let $G$ be a graph, $x\in V(G)$, and $Y\subseteq V(G) \backslash \{x \}$.
An $(x,Y)$-fan in $G$ is a set $\{P_1,\dots, P_k \}$ of paths in $G$ from $x$ to $Y$, such that $k = |Y|$ and $V(P_i)\cap V(P_j) = \{x \}$ for all $i\neq j$.

**Fan Lemma**:
?
Let $G$ be a $k$-connected graph, let $x\in V(G)$ and let $Y\subseteq V(G) \backslash \{x \}$ such that $|Y| = k$.
Then $G$ contains an $(x,Y)$-fan.

**Cycle Lemma**:
?
Let $G$ be a $k$-connected graph, where $k\geq 2$. Let $Y\subseteq V(G)$ where $|Y| = k$. Then there exists a cycle in $G$ containing all of $Y$.

**Corollary**: Every 3-connected graph contains {{a subdivision of $K_4$}}.