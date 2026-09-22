<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

Let $p(x)=\prod_{i=0}^n(x-x_i)$ be the monic node [polynomial](../../../../../polynomial-split.md). Suppose first that the quadrature is exact through degree $2n+1$. For any [polynomial](../../../../../polynomial-split.md) $r$ of degree at most $n$, $pr$ has degree at most $2n+1$, while every sampled value is zero. Exactness gives

$$
\int_a^b p(x)r(x)\,dx=\sum_i a_i p(x_i)r(x_i)=0.
$$

Thus $p$ is an [orthogonal polynomial](../../../../../orthogonal-polynomial.md) of degree $n+1$, proving necessity in the [orthogonal-node criterion for Gaussian quadrature](../../../../../orthogonal-node-criterion-for-gaussian-quadrature.md).

Conversely, suppose the nodes are the zeros of such a [polynomial](../../../../../polynomial-split.md). Rescale it to be monic without changing its zeros or orthogonality. For any $f$ of degree at most $2n+1$, [polynomial](../../../../../polynomial-split.md) division gives

$$
f=pq+r,\qquad\deg q\le n,\quad\deg r\le n.
$$

Orthogonality makes $\int pq=0$; the quadrature of $pq$ is zero because $p(x_i)=0$. The assumed degree-$n$ exactness applies to $r$, so

$$
\int_a^b f=\int_a^b r=\sum_i a_i r(x_i)=\sum_i a_i f(x_i).
$$

Hence **degree-$2n+1$ exactness is equivalent to orthogonal nodes**. The given distinct-zero property ensures the $n+1$ node values are independent interpolation data; the degree-$n$ exactness fixes the corresponding interpolatory weights. This is the construction of [Gaussian quadrature](../../../../../gaussian-quadrature.md).

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
