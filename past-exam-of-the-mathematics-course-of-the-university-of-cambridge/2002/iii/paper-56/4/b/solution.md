<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At the no-convection [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) $(a,b,c)=(0,0,0)$, one [eigenvalue](../../../../../../eigenvalue.md) is $-\zeta$ and the other two come from

$$
J_{ab}=\begin{pmatrix}\sigma(r-1)&-\sigma\zeta q\\1&-\zeta\end{pmatrix}.
$$

Their [trace](../../../../../../matrix-trace.md) and [determinant](../../../../../../determinant.md) are

$$
T=\sigma(r-1)-\zeta,\qquad D=\sigma\zeta(1+q-r).
$$

A zero [eigenvalue](../../../../../../eigenvalue.md) occurs at $r=1+q$. If $q<\zeta/\sigma$, the other two [eigenvalues](../../../../../../eigenvalue.md) are negative, and the stationary [bifurcation](../../../../../../bifurcation.md) is the pitchfork analyzed in part (c). For $q>\zeta/\sigma$ the transverse [eigenvalue](../../../../../../eigenvalue.md) is positive instead.

An imaginary pair occurs at $r=1+\zeta/\sigma$, provided $q>\zeta/\sigma$, because

$$
\omega_H^2=D=\sigma\zeta q-\zeta^2>0.
$$

The [trace](../../../../../../matrix-trace.md) crosses zero with [derivative](../../../../../../derivative.md) $\sigma>0$. The cubic coupling is nondegenerate here: at criticality, putting $K=\sigma\zeta q$ reduces the oscillatory variables to

$$
a''+\omega_H^2a=Kac,\qquad
c'=-\zeta c+\frac3K(\zeta a^2-aa').
$$

For $a=R\cos(\omega_H\tau)$, the forced second harmonic of $c$ has sine coefficient $9R^2\zeta\omega_H/[2K(\zeta^2+4\omega_H^2)]$. Averaging the [derivative](../../../../../../derivative.md) of $(a'^2+\omega_H^2a^2)/2$ consequently gives $-9\zeta\omega_H^2R^4/[8(\zeta^2+4\omega_H^2)]<0$. Thus the [Hopf bifurcation](../../../../../../hopf-bifurcation.md) is nondegenerate and supercritical.

The two thresholds meet at

$$
\boxed{q=\frac\zeta\sigma,\qquad r=1+\frac\zeta\sigma.}
$$

Here the planar block is nonzero but has [trace](../../../../../../matrix-trace.md) and [determinant](../../../../../../determinant.md) zero, while the third [eigenvalue](../../../../../../eigenvalue.md) remains negative. It is a reflection-symmetric double-zero, codimension-two point; the ordinary simple-eigenvalue reduction of part (c) is not valid there.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 56](../../../paper-56-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
