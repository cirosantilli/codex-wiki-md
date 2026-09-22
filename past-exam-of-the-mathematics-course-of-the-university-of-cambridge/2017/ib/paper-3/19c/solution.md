<h1 id="19c/solution">Solution</h1>

↑ **Parent:** [19C](../19c.md)

Let $x_1,\ldots,x_k$ be the distinct interior roots of $p_n$ where its sign changes, and put $q(x)=\prod_{j=1}^k(x-x_j)$. If $k<n$, [orthogonality](../../../../../orthogonal-vectors.md) gives $\int_a^bw p_nq=0$. But $p_nq$ has constant sign on $(a,b)$, apart from its isolated zeros, because every sign change has been canceled. It is not identically zero, and the positive weight makes its integral nonzero, a contradiction. Thus $k\ge n$. Degree $n$ forces exactly $n$ distinct simple roots, all inside $(a,b)$.

For distinct nodes, let $\ell_i(x)=\prod_{j\ne i}(x-c_j)/(c_i-c_j)$. [Lagrange interpolation polynomial](../../../../../lagrange-polynomial.md) gives $f=\sum_i f(c_i)\ell_i$ for every polynomial of degree at most $n-1$. Integrating this identity proves exactness with $b_i=\int_a^bw\ell_i$.

For the [Gaussian quadrature](../../../../../gaussian-quadrature.md) nodes, divide any $f\in\mathbb P_{2n-1}$ as $f=qp_n+r$, with $q,r\in\mathbb P_{n-1}$. The integral of $qp_n$ vanishes by [orthogonality](../../../../../orthogonal-vectors.md), and its nodal values vanish because $p_n(c_i)=0$. The remaining polynomial $r$ is integrated exactly by the preceding interpolation result. Hence

$$
\boxed{\text{the n-node Gaussian rule is exact through degree }2n-1.}
$$

Its weights are positive: exactness applied to $\ell_i^2$ gives $b_i=\int_a^bw\ell_i^2>0$.

Define the error functional $L(f)=\int_a^bw(x)f(x)\,dx-\sum_ib_if(c_i)$. It annihilates polynomials of degree at most $2n-1$. For $f\in C^{2n}[a,b]$, the [Peano kernel theorem](../../../../../peano-kernel-theorem.md) gives

$$
\boxed{L(f)=\int_a^bK(t)f^{(2n)}(t)\,dt,}
$$

where a formal [Peano kernel](../../../../../peano-kernel.md) with the normalization made explicit is

$$
K(t)=\frac1{(2n-1)!}\left[\int_t^bw(x)(x-t)^{2n-1}\,dx-\sum_i b_i(c_i-t)_+^{2n-1}\right].
$$

No evaluation of $K$ is needed. The supplied inner product presupposes an integrable positive weight on the finite interval, so the integral and point-evaluation error functional is bounded on continuous functions.

## ↑ Ancestors (10)

1. [19C](../19c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
