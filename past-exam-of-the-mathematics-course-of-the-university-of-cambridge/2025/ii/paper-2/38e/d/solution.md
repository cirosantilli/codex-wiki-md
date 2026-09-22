<h1 id="38e/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Define the [Ricci tensor](../../../../../../ricci-tensor.md) by contracting the first and third Riemann indices:

$$
R_{\alpha\gamma}=R^\mu{}_{\alpha\mu\gamma}.
$$

Contract the first Bianchi identity in its upper index and third lower index. The middle term vanishes by antisymmetry in the first pair, while antisymmetry in the final pair turns the last term into $-R_{\gamma\alpha}$. Thus

$$
R_{\alpha\gamma}-R_{\gamma\alpha}=0,
$$

so the Ricci tensor is symmetric.

For the stated constant-curvature form,

$$
\begin{aligned}
R_{\alpha\gamma}
&=g^{\mu\beta}R_{\mu\alpha\beta\gamma}
=(n-1)K g_{\alpha\gamma},\\
R&=g^{\alpha\gamma}R_{\alpha\gamma}
=n(n-1)K.
\end{aligned}
$$

The [contracted Bianchi identity](../../../../../../contracted-bianchi-identity.md) is

$$
\nabla^\alpha R_{\alpha\beta}=\frac12\nabla_\beta R.
$$

Using $\nabla g=0$ gives

$$
(n-1)\partial_\beta K
=\frac12n(n-1)\partial_\beta K,
$$

or

$$
\frac{(n-1)(n-2)}2\,\partial_\beta K=0.
$$

In four dimensions,

$$
\boxed{R_{\alpha\beta}=3Kg_{\alpha\beta},
\qquad R=12K,
\qquad K\text{ is constant}.}
$$

More generally, $K$ is constant for every $n>2$. In dimension $n=2$, the contracted Bianchi identity gives no such conclusion, and the Gaussian curvature may vary from point to point.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [38E](../../38e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
