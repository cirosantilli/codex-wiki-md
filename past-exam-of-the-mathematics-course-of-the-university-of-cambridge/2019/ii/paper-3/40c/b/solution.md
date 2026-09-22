<h1 id="40c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $L=[1,-2,1]$ be the symmetric Dirichlet second-difference matrix on the $M$ interior points. The method is

$$
\left(aI-\frac{\mu-c}{4}L\right)u^{n+1}
=\left(aI+\frac{\mu+c}{4}L\right)u^n.
$$

The orthogonal sine vectors diagonalize $L$, with eigenvalues

$$
\ell_j=-4s_j,
\qquad
s_j=\sin^2\left(\frac{j\pi}{2(M+1)}\right),
\qquad j=1,\ldots,M.
$$

Because the two time-level matrices are real symmetric polynomials in the same symmetric matrix, they share this orthonormal eigenbasis. Whenever the left matrix is invertible, the amplification matrix is therefore normal, so its Euclidean operator norm is the largest modulus of its eigenvalues. The $j$th [amplification factor](../../../../../../amplification-factor.md) is

$$
G_j=\frac{a-(\mu+c)s_j}{a+(\mu-c)s_j}.
$$

For the physical Courant number $\mu>0$,

$$
|a+(\mu-c)s|^2-|a-(\mu+c)s|^2
=4\mu s(a-cs).
$$

Hence $|G_j|\leq1$ exactly when $a-cs_j\geq0$. Requiring this uniformly for every mesh, whose values $s_j$ become dense in $(0,1)$, gives

$$
a-cs\geq0\quad(0\leq s\leq1).
$$

Equivalently, $a\geq0$ and $c\leq a$. Under these inequalities the denominator is nonzero for every $0<s<1$: if $c\leq\mu$ this is immediate, while if $c>\mu$ then $a\geq c$ gives $a+(\mu-c)s\geq a+\mu-c\geq\mu>0$. Thus the necessary and sufficient mesh-uniform stability conditions are

$$
\boxed{\mu>0,\qquad a\geq0,\qquad c\leq a.}
$$

This is the [stability of a two-parameter implicit-explicit diffusion scheme](../../../../../../stability-of-a-two-parameter-implicit-explicit-diffusion-scheme.md). If consistency with the stated diffusion equation is also required, comparison of the leading Taylor terms gives $ak u_t=(k/2)u_{xx}+o(k)$, so $a=1/2$ and the stable consistent family has $c\leq1/2$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [40C](../../40c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
