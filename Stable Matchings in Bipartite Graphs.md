**Preference List**
?
Let $G$ be a bipartite graph with vertex classes $X$ and $Y$. A set $L$ of **preference lists** for $G$ is a set of linear orders $L(v)$ on $N(v)$ for each $v\in X\cup Y$.

**Stable Matching**
?
Let $G$ be bipartite. A matching $M$ in $G$ with preference list $L$ is called **stable** if for every edge $xy\in G\backslash M$, either:
- $x$ is matched by $M$ to a neighbour that $x$ prefers over $y$, that is, $xy'\in M$ for some $y'>y$ in $L(x)$.
- $y$ is matched by $M$ to a neighbour that $y$ prefers over $x$, that is, $x'y\in M$ for some $x'>x$ in $L(y)$.
- *Note*: not every stable matching is maximal.

**Gale-Shapley Algorithm**: Consider a bipartite graph $GA$, the Gale-Shapley algorithm outputs a stable matching $M$ constructed by,
?
```
M <- empty set
for x in X:
	K(x) <- L(x)

while not (for all x in X, K(x) == empty OR x saturated by M):
	# find x to propose
	x <- element of X s.t. x is M-exposed and K(x) = empty 
	y <- max in K(x)
	if yx' in M and y prefers x to x':
		# x is preferred to x'
		M = M\{yx'} union {yx}
	else:
		# y is M-exposed
		M = M union {xy}
	K(x) = K(x) \ {y}
 
return M	
```

**Theorem** Unique Stable Matching Vertex Saturation:
?
Let $G$ be a bipartite graph with preference lists $L$. Then all stable matchings in $G$ saturate the same set of vertices.

**Corollary**: All stable matchings in ($G,L$) have the same size.

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


