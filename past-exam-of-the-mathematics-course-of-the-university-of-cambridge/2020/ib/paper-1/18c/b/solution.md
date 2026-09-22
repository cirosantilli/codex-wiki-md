<h1 id="18c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For fixed [interpolation nodes](../../../../../../interpolation-node.md) $c_0,\ldots,c_{s-1}$, interpolate any $p\in\mathbb P_{s-1}[x]$ as

$$
p(x)=\sum_{k=0}^{s-1}p(c_k)\ell_k(x),
\qquad
\ell_k(x)=\prod_{j\ne k}\frac{x-c_j}{c_k-c_j}.
$$

Integrating shows that the unique weights making the [quadrature rule](../../../../../../quadrature-rule.md) exact through degree $s-1$ are

$$
\boxed{w_k=\int_a^b\ell_k(x)\,dx
=\int_a^b\prod_{j\ne k}\frac{x-c_j}{c_k-c_j}\,dx}.
$$

Now let the nodes be the zeros of the degree-$s$ [orthogonal polynomial](../../../../../../orthogonal-polynomial.md) $q_s$. Given any $p\in\mathbb P_{2s-1}[x]$, [polynomial division](../../../../../../polynomial-division.md) gives

$$
p=q_sh+r,
\qquad \deg h\le s-1,quad \deg r\le s-1.
$$

Orthogonality gives $\int_a^bq_sh=0$, while $q_s(c_k)=0$ makes the quadrature sum for $q_sh$ vanish. The rule is already exact on $r$, so it is exact on $p$. This is the defining precision property of [Gaussian quadrature](../../../../../../gaussian-quadrature.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [18C](../../18c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
