<h1 id="2h/solution">Solution</h1>

↑ **Parent:** [2H](../2h.md)

The [Legendre polynomial](../../../../../legendre-polynomial.md) $p_n$ is [orthogonal](../../../../../orthogonal-polynomial.md) on $[-1,1]$ to every polynomial of degree below $n$. Suppose it changes sign at only $r<n$ distinct interior points $x_1,\ldots,x_r$, and put

$$
q(x)=\prod_{j=1}^r(x-x_j),
$$

choosing its overall sign so that $p_nq\ge0$ on $[-1,1]$. This product is positive except at finitely many points, so

$$
\int_{-1}^1p_n(x)q(x)\,dx>0,
$$

contradicting orthogonality because $\deg q=r<n$. Thus $p_n$ has at least $n$ sign-changing roots in $(-1,1)$; its degree is $n$, so these are all its roots and they are distinct.

For arbitrary distinct nodes $x_1,\ldots,x_n$, let

$$
L_i(t)=\prod_{j\ne i}\frac{t-x_j}{x_i-x_j}
$$

be the [Lagrange basis polynomials](../../../../../lagrange-polynomial.md). Every polynomial $P$ of degree below $n$ satisfies $P(t)=\sum_iP(x_i)L_i(t)$, so the required weights exist and are

$$
A_i=\int_{-1}^1L_i(t)\,dt.
$$

They are unique because applying any such formula to $P=L_i$ recovers $A_i$.

Now assume exactness for every $P$ of degree below $2n$ and define $Q(t)=\prod_i(t-x_i)$. For every polynomial $R$ of degree below $n$, the product $QR$ has degree below $2n$ and vanishes at every node. Therefore

$$
\int_{-1}^1Q(t)R(t)\,dt=0.
$$

There is a unique monic polynomial of degree $n$ orthogonal to all lower-degree polynomials, so $Q$ is the monic normalization of $p_n$ and the $x_i$ are precisely the roots of $p_n$. Taking $P=1$ gives

$$
\boxed{\sum_{i=1}^nA_i=2}.
$$

Finally $L_i^2$ has degree $2n-2$, so exactness gives

$$
A_i=\sum_jA_jL_i(x_j)^2
=\int_{-1}^1L_i(t)^2\,dt>0.
$$

These are the positive weights of [Gaussian quadrature](../../../../../gaussian-quadrature.md).

## ↑ Ancestors (10)

1. [2H](../2h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
