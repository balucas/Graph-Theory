
**X-optimal stable matching**
?
An $X$ optimal stable matching is a stable matching $M^*$ such that, for every stable matching $M$ and every $x \in X$, if $xy \in M$ then $\exists y' \in Y$ such that $xy' \in M^*$ and $y' \geq y$ in $L(x)$.
In other words, $x$ obtains the best possible partner in $M*$ that it could in any stable matching.

**X-pessimal stable matching**
?
An $X$ pessimal stable matching is a stable matching $M^*$ such that, for every stable matching $M$ and every $x \in X$, if $xy \in M$ then $\exists y' \in Y$ such that $xy' \in M^*$ and $y' \leq y$ in $L(x)$.
In other words, $x$ obtains the worst possible partner in $M*$ that it could in any stable matching.

**Gale Shapley Algorithm optimality**
?
Let $G$ be a bipartite graph with preference lists $L$ and vertex classes $X$ and $Y$. Then, the Gale-Shapley matching (with $X$ side proposing), is $X$-optimal.

**Gale Shapley Algorithm uniqueness**
?
Let $G$ be a bipartite graph with preference lists $L$ and vertex classes $X$ and $Y$. Then, the Gale-Shapley algorithm will produce a unique matching independent of the order in which proposals are made.
