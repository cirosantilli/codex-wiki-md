<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $f(x)=\sum_{j=0}^d a_jx^j$. For $n\ge\max(1,d)$, express $f$ in the [Bernstein basis](../../../../../../bernstein-basis.md) as $f=\sum_{k=0}^n\beta_{k,n}b_{k,n}$, where $b_{k,n}=\binom nkx^k(1-x)^{n-k}$. Its precomputed coefficients are

$$
\beta_{k,n}=\sum_{j=0}^{\min(k,d)}a_j\frac{(k)_j}{(n)_j},
$$

with the ratio for $j=0$ interpreted as one. The identity follows from $x^j=\sum_k[(k)_j/(n)_j]b_{k,n}$, obtained by the [binomial theorem](../../../../../../binomial-theorem.md).

At this level solve the [linear program](../../../../../../linear-programming.md)

$$
\boxed{v_n=\max_{\lambda\in\mathbb R}\{\lambda:\lambda\le\beta_{k,n},\quad0\le k\le n\}=\min_k\beta_{k,n}.}
$$

There are exactly $n+1$ inequalities. Equivalently, $f-\lambda$ must have nonnegative coefficients in the unnormalized basis; its coefficients are $\binom nk(\beta_{k,n}-\lambda)$. Since the basis functions are nonnegative and sum to one, every feasible $\lambda$ satisfies $\lambda\le f(x)$ for all $x\in[0,1]$, so $v_n\le f_{\min}$.

[Degree elevation of Bernstein coefficients](../../../../../../degree-elevation-of-bernstein-coefficients.md) gives, for $1\le k\le n$,

$$
\beta_{k,n+1}=\frac{k}{n+1}\beta_{k-1,n}+\left(1-\frac{k}{n+1}\right)\beta_{k,n},
$$

with endpoint coefficients unchanged. These [convex combinations](../../../../../../convex-combination.md) imply $v_{n+1}\ge v_n$.

To cover every positive index even when $d>1$, put $\ell=a_0-\sum_{j=1}^d|a_j|$. For $1\le n<d$, use the one-inequality LP $\max\{\lambda:\lambda\le\ell\}$, giving $v_n=\ell$. This is a lower bound on $f$; moreover the explicit coefficient formula has all its factorial ratios in $[0,1]$, so $\beta_{k,d}\ge\ell$. Thus the transition to level $d$ is also monotone and every level respects the requested bound of at most $n+1$ inequalities. Constants are handled by the main formula at all positive indices.

Finally, for every $\epsilon>0$, $f-(f_{\min}-\epsilon)$ is strictly positive on the interval. Part (c) supplies a nonnegative-coefficient representation at some degree, and degree elevation preserves it at every higher degree. Hence eventually $v_n\ge f_{\min}-\epsilon$. Combining with the upper bound proves the [Bernstein linear programming hierarchy for polynomial minimization](../../../../../../bernstein-linear-programming-hierarchy-for-polynomial-minimization.md):

$$
\boxed{v_1\le v_2\le\cdots\le\min_{x\in[0,1]}f(x),\qquad v_n\longrightarrow\min_{x\in[0,1]}f(x).}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
