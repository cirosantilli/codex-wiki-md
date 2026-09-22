<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the compatible metrics $g_\Sigma(\cdot,\cdot)=\omega_\Sigma(\cdot,j\cdot)$ and $g_X(\cdot,\cdot)=\omega_X(\cdot,J\cdot)$. The energy of a smooth map is

$$
E(u)=\frac12\int_\Sigma|du|^2\,\omega_\Sigma.
$$

It is a [J-holomorphic curve](../../../../../pseudoholomorphic-curve.md) when $du\circ j=J\circ du$. Splitting $du$ into its complex-linear and complex-antilinear parts gives the [Energy identity for a J-holomorphic curve](../../../../../energy-identity-for-a-j-holomorphic-curve.md)

$$
E(u)=\int_\Sigma u^*\omega_X+	ext{a nonnegative multiple of }\|\bar\partial_Ju\|_{L^2}^2.
$$

The first term depends only on the homology class. It follows that a J-holomorphic map minimizes energy among all maps in its homology class.

One [Monotonicity theorem for a J-holomorphic curve](../../../../../monotonicity-theorem-for-a-j-holomorphic-curve.md) says that a nonconstant J-holomorphic curve through the center of a sufficiently small radius-$\rho$ ball, with boundary outside that ball, has area at least $c\rho^2$; in the standard complex ball one may take the sharp value $\pi\rho^2$. The [Gromov non-squeezing theorem](../../../../../non-squeezing-theorem.md) says

$$
B^{2n}(R)\hookrightarrow B^2(r)\times\mathbb R^{2n-2}
\quad\Longrightarrow\quad R\leq r.
$$

Write $\mathbb R^4=T^*\mathbb R^2$ with coordinates $(q,p)$ and form $dq_1\wedge dp_1+dq_2\wedge dp_2$. For $c>0$, the graph

$$
L_c=\{(q,cq):q\in\mathbb R^2\}
$$

is a [Lagrangian subspace](../../../../../lagrangian-subspace.md). Points of $L_c\cap B(R)$ have $|q|\leq R/\sqrt{1+c^2}$. Choose $c$ so large that

$$
\frac{2R}{\sqrt{1+c^2}}+2\varepsilon<1.
$$

Then no two points of the $\varepsilon$-neighborhood of $L_c\cap B(R)$ differ by a nonzero vector $(m,0)$ with $m\in\mathbb Z^2$, so quotienting $q$ modulo $\mathbb Z^2$ is injective there.

Relative to the Lagrangian splitting $L_c\oplus JL_c$, the map $(v,w)\mapsto(\lambda v,\lambda^{-1}w)$ is symplectic. It sends $B^4(r)$ into the indicated long thin neighborhood whenever

$$
\lambda r<R,
\qquad
r/\lambda<\varepsilon.
$$

These inequalities are compatible when $R>r^2/\varepsilon$. Taking such an $R$ and then the quotient constructs the [arbitrarily large symplectic balls in a cotangent cylinder](../../../../../arbitrarily-large-symplectic-balls-in-a-cotangent-cylinder.md):

$$
\boxed{B^4(r)\hookrightarrow T^2\times\mathbb R^2\text{ for every }r>0.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 146](../../paper-146-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
