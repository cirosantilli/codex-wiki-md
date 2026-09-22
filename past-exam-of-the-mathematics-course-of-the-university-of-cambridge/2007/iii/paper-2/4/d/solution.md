<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At a primitive cube [root of unity](../../../../../../root-of-unity.md), $[1]=1$, $[2]=-1$, $[3]=0$. In the degree-three [quantum plane](../../../../../../quantum-plane.md) [module](../../../../../../module-mathematics.md), put $z_0=x^3$, $z_1=x^2y$, $z_2=xy^2$, $z_3=y^3$. The complete actions are

$$
\begin{array}{c|rrrr}
&z_0&z_1&z_2&z_3\\\hline
K&z_0&qz_1&q^{-1}z_2&z_3\\
E&0&z_0&-z_1&0\\
F&0&-z_2&z_3&0
\end{array}.
$$

Hence $W=\langle z_0,z_3\rangle$ is a two-dimensional trivial [submodule](../../../../../../submodule.md); every line in $W$ is a [simple module](../../../../../../irreducible-module.md). The quotient by $W$ is a two-dimensional [simple module](../../../../../../irreducible-module.md), with distinct $K$ [eigenvalues](../../../../../../eigenvalue.md) $q,q^{-1}$ and nonzero maps connecting its two [weight spaces](../../../../../../weight-space.md).

Let $S$ be a [simple module](../../../../../../irreducible-module.md) that is a [submodule](../../../../../../submodule.md) of this cubic component. If $S\cap W\ne0$, simplicity makes $S\subseteq W$, so $S$ is one of its lines. If $S\cap W=0$, the quotient map injects $S$ into the simple quotient. Its nonzero image is the entire quotient, so $\dim S=2$. Since $K$ is diagonalizable, such an $S$ must contain the unique $q$ [weight space](../../../../../../weight-space.md) $\mathbb C z_1$. But $Ez_1=z_0\ne0$, which then belongs to $S\cap W$, a contradiction. Therefore the [cubic-root quantum-plane socle](../../../../../../cubic-root-quantum-plane-socle.md) gives the complete answer:

$$
\boxed{S=\mathbb C(\alpha x^3+\beta y^3),\qquad(\alpha,\beta)\ne(0,0).}
$$

All simple [submodules](../../../../../../submodule.md) lie in the two-dimensional $W$, so their sum cannot equal the four-dimensional cubic component. **It is not a direct sum of simple modules.** The obstruction is the nonzero extension to the simple two-dimensional quotient, not a failure of that quotient to be simple.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
