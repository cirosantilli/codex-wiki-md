<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the adult-survival [annual pulse-breeding predator-prey model](../../../../../../annual-pulse-breeding-predator-prey-model.md), a positive annual [fixed point](../../../../../../fixed-point.md) exists when $r>1$ and $0<s<1$:

$$
X_* =\frac{1-s}{sb},\qquad Y_* =\frac{\log r}{\kappa}.
$$

At this point the [Jacobian matrix](../../../../../../jacobian-matrix.md) is

$$
J_*=
\begin{pmatrix}
1&-\kappa X_*\\sbY_*&1-(1-s)\log r
\end{pmatrix},
\qquad
\boxed{\det J_*=1,\quad \operatorname{tr}J_*=2-(1-s)\log r.}
$$

If $0<(1-s)\log r<4$, the two [eigenvalues](../../../../../../eigenvalue.md) are a [complex conjugate](../../../../../../complex-conjugate.md) pair of [moduli](../../../../../../modulus.md) one. The annual samples show linearly neutral seasonal oscillations. If $(1-s)\log r>4$, they form a reciprocal negative real pair and the [fixed point](../../../../../../fixed-point.md) is a [saddle fixed point of a map](../../../../../../saddle-fixed-point-of-a-map.md). Equality at four is a degenerate boundary needing nonlinear analysis. For replacement rather than surviving adults the same calculation gives [trace](../../../../../../matrix-trace.md) $2-\log r$ and [determinant](../../../../../../determinant.md) one.

The absence of an attracting annual cycle is stronger than a linear observation. Put $u=\log X$, $v=\log Y$. The update becomes

$$
u'=u+\log r-\kappa e^v,
\qquad v'=v+\log s+\log(1+be^{u'}).
$$

It is the composition of two [nonlinear shear maps](../../../../../../nonlinear-shear-map.md), each of [determinant](../../../../../../determinant.md) one: an [area-preserving seasonal predator-prey map](../../../../../../area-preserving-seasonal-predator-prey-map.md). No isolated positive [periodic orbit](../../../../../../periodic-orbit.md) has an open attracting basin. Neutral linear oscillations alone also do not prove nonlinear stability at every resonance. In particular, this density-independent model does not select an [asymptotically stable](../../../../../../asymptotic-stability.md) oscillation amplitude.

The [Nicholson-Bailey model](../../../../../../nicholson-bailey-model.md) instead counts [parasitoid](../../../../../../parasitoid.md) offspring from attacked [hosts](../../../../../../host-biology.md):

$$
X'=rXe^{-\kappa Y},\qquad Y'=cX(1-e^{-\kappa Y}).
$$

Its positive [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) has $Y_*=\log r/\kappa$ and $X_*=Y_*/[c(1-1/r)]$. Its [Jacobian matrix](../../../../../../jacobian-matrix.md) has

$$
\det J_* =\frac{r\log r}{r-1}>1,
\qquad \operatorname{tr}J_*=1+\frac{\log r}{r-1}<2.
$$

Since the [determinant](../../../../../../determinant.md) exceeds one while the positive [trace](../../../../../../matrix-trace.md) is below two, the [eigenvalues](../../../../../../eigenvalue.md) are complex with [moduli](../../../../../../modulus.md) greater than one: [instability of the Nicholson-Bailey equilibrium](../../../../../../instability-of-the-nicholson-bailey-equilibrium.md) produces outward oscillations near it. The two maps share an exponential prey-survival factor but have different reproduction laws and stability properties.

<a id="1/b/image-neutral-seasonal-predator-prey-oscillations-compared-with-the-unstable-nicholson-bailey-equilibrium"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-52-seasonal-orbits.png)

**[Figure 1](#1/b/image-neutral-seasonal-predator-prey-oscillations-compared-with-the-unstable-nicholson-bailey-equilibrium). Neutral seasonal predator-prey oscillations compared with the unstable Nicholson-Bailey equilibrium**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
