<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [lazy Markov chain](../../../../../../lazy-markov-chain.md) has holding probability $1/2$ and [transition probability](../../../../../../transition-probability.md) $1/(2n)$ to each neighbour in the [hypercube graph](../../../../../../hypercube-graph.md). Its [stationary distribution](../../../../../../stationary-distribution.md) is $\pi(x)=2^{-n}$ by symmetry.

For $(x,y)$ choose the [path](../../../../../../continuous-path.md) changing the differing coordinates in increasing order. Its length is at most $n$. Fix a directed [edge](../../../../../../edge-of-a-graph.md) $(u,u^{(k)})$ that flips coordinate $k$. A [path](../../../../../../continuous-path.md) uses this [edge](../../../../../../edge-of-a-graph.md) exactly when $x_k=u_k$, $y_k=-u_k$, $y_j=u_j$ for $j<k$, and $x_j=u_j$ for $j>k$. The coordinates $x_j$ for $j<k$ and $y_j$ for $j>k$ are free. Thus exactly $2^{n-1}$ ordered pairs use it, while

$$
Q(u,u^{(k)})=\frac{2^{-n}}{2n},\qquad
\sum_{(x,y):e\in\eta_{xy}}\pi(x)\pi(y)=2^{n-1}2^{-2n}=2^{-n-1}.
$$

The unweighted load divided by capacity equals $n$; multiplying by the maximum length yields $\rho\leq n^2$. The [canonical paths Poincare bound](../../../../../../canonical-paths-poincare-bound.md) therefore proves the slightly stronger $\operatorname{Var}_\pi(f)\leq n^2\mathcal E(f,f)$, and in particular the requested

$$
\boxed{\operatorname{Var}_\pi(f)\leq2n^2\mathcal E(f,f),\qquad\gamma\geq\frac1{2n^2}.}
$$

One can keep the actual lengths: among these $2^{n-1}$ pairs, coordinate $k$ always differs, and each of the other $n-1$ coordinates differs for half the pairs. Their mean [path](../../../../../../continuous-path.md) length is $(n+1)/2$, giving exact congestion $\rho=n(n+1)/2$. This refinement still has order $n^2$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
