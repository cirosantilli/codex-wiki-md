<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a nonzero [holomorphic vector bundle](../../../../../../holomorphic-vector-bundle.md) $F$ on the curve, its [degree of a holomorphic vector bundle](../../../../../../degree-of-a-holomorphic-vector-bundle.md) and [slope of a holomorphic vector bundle](../../../../../../slope-of-a-holomorphic-vector-bundle.md) are

$$
\deg F=\deg\det F,\qquad \mu(F)=\frac{\deg F}{\operatorname{rank}F}.
$$

We obtain a bound independent of the particular [holomorphic subbundle](../../../../../../holomorphic-subbundle.md) by fixing a [Hermitian metric on a holomorphic vector bundle](../../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md) $E$ once and for all. Let $D_E$ be its [Chern connection](../../../../../../chern-connection.md), $F_E=D_E^2$ its [Chern curvature](../../../../../../chern-curvature.md), and $\omega$ any positive area form on the [compact Riemann surface](../../../../../../compact-riemann-surface.md). Write

$$
iF_E=K\omega.
$$

Here $K$ is a smooth Hermitian endomorphism of $E$. By [compactness](../../../../../../compact-space.md), its largest eigenvalue is bounded above by some finite constant $C$ on the whole curve.

Let $F\subseteq E$ be a [holomorphic subbundle](../../../../../../holomorphic-subbundle.md) of positive rank $r$, with the induced metric. Use the smooth [orthogonal splitting of a vector subbundle](../../../../../../orthogonal-splitting-of-a-vector-subbundle.md) $E=F\oplus F^\perp$. In this splitting the connection has block form

$$
D_E=\begin{pmatrix}D_F&-B^\dagger\\B&D_Q\end{pmatrix},
$$

where $D_F$ is the [projected Chern connection](../../../../../../projected-chern-connection.md) and $B$ is the [second fundamental form of a holomorphic subbundle](../../../../../../second-fundamental-form-of-a-holomorphic-subbundle.md). The latter has type $(1,0)$: the $(0,1)$ part of $D_E$ preserves the holomorphic subbundle. The adjoint $B^\dagger$ includes conjugation of the form factor and has type $(0,1)$. Squaring this block matrix gives

$$
(F_E)_{11}=F_F-B^\dagger\wedge B,\qquad F_F=(F_E)_{11}+B^\dagger\wedge B.
$$

This derives the [curvature formula for a holomorphic subbundle](../../../../../../curvature-formula-for-a-holomorphic-subbundle.md) in the column-vector convention used here. Locally write $B=b\,dz$. Then

$$
B^\dagger\wedge B=-b^\dagger b\,dz\wedge d\bar z.
$$

The [degree of a holomorphic vector bundle](../../../../../../degree-of-a-holomorphic-vector-bundle.md) is the trace-curvature integral, since the trace is the curvature of the [determinant line bundle](../../../../../../determinant-line-bundle.md). Hence

$$
\deg F=\frac{i}{2\pi}\int_X\operatorname{tr}F_F
=\frac{1}{2\pi}\int_X\operatorname{tr}(P_FK|_F)\,\omega
-\frac{1}{2\pi}\int_X i\operatorname{tr}(b^\dagger b)\,dz\wedge d\bar z.
$$

The last integrand is a nonnegative real two-form and is independent of the local unitary frame and coordinate. Since $K\le C I_E$, the compressed trace is at most $rC$ pointwise. Therefore

$$
\deg F\le\frac{rC}{2\pi}\int_X\omega,
\qquad
\boxed{\mu(F)\le\frac{C}{2\pi}\int_X\omega.}
$$

This is the [subbundle slope bound from ambient Chern curvature](../../../../../../subbundle-slope-bound-from-ambient-chern-curvature.md). The right side depends only on $E$ and the initially chosen metrics, and is finite. It proves the requested uniform upper bound for every positive-rank subbundle, without assuming any stability property of $E$ or using a bound that depends on $F$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
