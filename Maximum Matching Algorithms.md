**Shrinkable Cycles**
?
Let $G$ be a graph with matching $M$. An odd cycle $C$ is shrinkable with respect to $M$ if, when $C$ has length $2k+1$:
$|M \cap E(C)| =k$, and $C$ contains an $M$ exposed vertex

**Cycle Shrinking Lemma**
?
Let $G$ be a graph with matching $M$. Let $C$ be a cycle with length $2k+1$ that is shrinkable with respect to $M$. The graph $G'$ obtained from $G$ by contracting all edges of $C$ has maximum matching $M' = M \backslash E(C)$ if and only if $M$ is maximum in $G$.

**M alternating Trees**
?
Let $M$ be a matching in a graph $G$, an $M$-alternating tree in $G$ is a subgraph, $T$ of $G$ such that, 
- $T$ is a tree,
- $T$ contains exactly one $M$ exposed vertex, $s$ called the root of $T$
- Each edge of $T$ at an odd distance in $T$ from the root $s$, is in $M$
- Each vertex of $T$ at an odd distance in $T$ from the root $s$, called inner vertices of $T$ (denoted $I(T)$) have degree exactly 2 in $T$.
- The remaining vertices (of even distance from $s$) are called outer vertices (denoted $O(T)$). Note $s \in O(T)$

**M alternating forest**
?
Let $M$ be a matching in a graph $G$, an $M$ alternating forest in $G$ is a subgraph $F$ of $G$ such that every component of $F$ is an $M$ alternating tree. The set of inner and outer vertices of $F$, $I(F)$, $O(F)$, is the union of the inner and outer vertices of all components of $F$.
Such an $M$ alternating is maximal if it is not contained in any larger $M$ alternating forest in $G$.

**Maximal M alternating forest lemma 1**:
Let $M$ be a matching in a graph $G$ and $F$ a maximal $M$ alternating forest. Suppose there is no edge of $G$ joining two outer vertices of $F$. Then, {{$M$ is maximum in $G$}}.

**Maximal M alternating forest lemma 2**:
Let $M$ be a matching in a graph $G$ and $F$ a maximal $M$ alternating forest. Suppose there is an edge of $G$ joining two outer vertices of $F$ in **different** components. Then, {{this edge lies in an $M$ augmenting path}}.

**Maximal M alternating forest lemma 3**:
Let $M$ be a matching in a graph $G$ and $F$ a maximal $M$ alternating forest. Suppose there is an edge of $G$ joining two outer vertices of $F$ in the **same** component. Then, {{there exists a matching $\overline{M}$ in $G$ where $|M| = |\overline{M}|$ and an odd cycle $C$ in $G$ that is shrinkable with respect to $\overline{M}$ }}.

**Edmonds' Algorithm for Maximum Matching**
?
Begin with a graph $G$ and end with a maximum matching of $G$.
- Begin with $G$ and matching $M$.
- Begin constructing an $M$ alternating forest $F$ in $G$

Case 1: If there is no edge of $G$ joining two outer vertices of $F$, then $M$ is maximum.
Case 2: If we find an edge $xy \in E(G)$ such that for $x,y \in O(T)$ for some component $T$ of $F$, go back to beginning with input $G-C$ and $\overline{M} \backslash E(C)$ 
Case 3: If we find an edge $xy \in E(G)$ such that $x \in O(T_1)$, $y \in O(T_2)$ for $T_1 \neq T_2$, replace $M$ with $M \Delta E(P)$, expand all shrunken odd cycles and add corresponding edges to $M$ to obtain a larger matching $M'$ in the original graph $G$. Go back to beginning with input $G$ and matching $M'$

**f-factor**: Let $G$ be a graph and consider the function $f:V(G) \rightarrow \{0,1,2,...\}$. An $f$ factor in $G$ is a spanning subgraph, $H$ of $G$ such that $deg_H(v) = f(v)$ for all $v \in V(G) = V(H)$

**Tutte's $f$ factor graph theorem**: 
For a graph $G$ and function $f: V(G) \rightarrow \{0,1,2,...\} such that $deg_G(v) \leq f(v)$ for all $v \in V(G)$, the graph $H(G,f)$ as defined above, has a perfect matching if and only if {{$G$ has an $f$-factor}}

**Petersen's Theorem**:: Every regular graph of even positive degree has a 2-factor


