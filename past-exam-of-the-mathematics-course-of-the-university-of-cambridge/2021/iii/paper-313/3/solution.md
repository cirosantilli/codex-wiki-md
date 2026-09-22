<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For the curvature two-form

$$
F=dA+A\wedge A,
$$

use the normalization

$$
\boxed{C_2=\frac1{8\pi^2}\operatorname{Tr}(F\wedge F)}
$$

for the [Second Chern form](../../../../../second-chern-form.md). Graded cyclicity of the trace gives $\operatorname{Tr}(A^{\wedge4})=0$ and

$$
\operatorname{Tr}(F\wedge F)
=\operatorname{Tr}\left(dA\wedge dA
+2dA\wedge A\wedge A\right).
$$

On the other hand,

$$
d\operatorname{Tr}(A\wedge dA)=\operatorname{Tr}(dA\wedge dA),
$$

and

$$
d\operatorname{Tr}(A\wedge A\wedge A)
=3\operatorname{Tr}(dA\wedge A\wedge A).
$$

Thus the coefficient in the [Chern-Simons 3-form](../../../../../chern-simons-3-form.md) must be

$$
\boxed{c=\frac23},
$$

and

$$
\boxed{C_2=dY,\qquad
Y=\frac1{8\pi^2}\operatorname{Tr}\left(
A\wedge dA+\frac23A\wedge A\wedge A\right)}.
$$

For the gauge transformation $A'=gAg^{-1}-dg\,g^{-1}$, use $d(g^{-1})=-g^{-1}(dg)g^{-1}$ and the [Maurer-Cartan equation](../../../../../maurer-cartan-equation.md). Expanding $dA'+A'\wedge A'$ makes the terms linear and quadratic in $dg\,g^{-1}$ cancel, leaving

$$
\boxed{F'=gFg^{-1}}.
$$

Invariance of the matrix trace under conjugation then gives

$$
\boxed{C_2'=\frac1{8\pi^2}\operatorname{Tr}(gFg^{-1}\wedge gFg^{-1})=C_2}.
$$

A [Yang-Mills instanton](../../../../../yang-mills-instanton.md) on $\mathbb R^4$ has finite Euclidean action, smooth curvature in the interior, and $F\to0$ sufficiently rapidly at infinity. Its connection therefore approaches a pure gauge on the asymptotic three-sphere,

$$
A\longrightarrow-dg\,g^{-1}
$$

up to a decaying correction, for a map $g:S^3_\infty\to SU(2)$. By [Stokes theorem](../../../../../stokes-theorem.md),

$$
k=\int_{\mathbb R^4}C_2
=\int_{S^3_\infty}Y.
$$

Writing $\theta=dg\,g^{-1}$ gives $d\theta=\theta\wedge\theta$ and, for $A=-\theta$,

$$
Y=\frac1{24\pi^2}\operatorname{Tr}(\theta^{\wedge3}).
$$

Hence the [instanton number as a winding number at infinity](../../../../../instanton-number-as-a-winding-number-at-infinity.md) is

$$
\boxed{k=\frac1{24\pi^2}\int_{S^3_\infty}
\operatorname{Tr}\left[(dg\,g^{-1})^{\wedge3}\right]\in\mathbb Z}.
$$

Under $SU(2)\cong S^3$, this integer is the [degree of a map between oriented manifolds](../../../../../degree-of-a-map-between-oriented-manifolds.md) $g:S^3\to S^3$. Reversing the trace or orientation convention reverses the displayed sign.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 313](../../paper-313-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
