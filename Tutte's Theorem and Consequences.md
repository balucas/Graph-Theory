**Tutte's Theorem**: A graph $G$ has a perfect matching if and only if {{for every $T \subseteq V(G)$, we have that $|T| \geq odd(G-T)$}}

**Equal parity**: Let $G$ be a graph such that $|V(G)|$ is even. Then, $\forall T \subseteq V(G)$, we have that {{$odd(G-T) \equiv |T|\pmod 2$}}

**Bridge**: In a connected graph $G$, $e \in E(G)$ is a bridge if $G \backslash e$ is disconnected.

**Petersen's Theorem**:
?
Let $G$ be a connected cubic graph with at most 2 bridges. Then $G$ has a perfect matching.

**Defect version of Tutte's Theorem**
?
Let $G$ be a graph. Let $\displaystyle d := \max_{T \subseteq V(G)} \{odd(G-T)-|T|\}$
Then, $G$ has a matching that saturates at least $|V(G)|-d$ vertices.

**Tutte-Berge Formula**
?
Let $G$ be a graph. Let $\displaystyle d := \max_{T \subseteq V(G)} \{odd(G-T)-|T|\}$
Then, $\nu(G) = \frac{|V(G)| - d}{2}$








