<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The required anomaly cancellation depends on the exact [Eisenstein series of weight two](../../../../../../eisenstein-series-of-weight-two.md) law

$$
E_2(\gamma\tau)=j^2E_2(\tau)+\frac{12c}{2\pi i}j,\qquad j=c\tau+d.
$$

Here is a way to establish it without assuming that $E_2$ is a [modular form](../../../../../../modular-form.md). The lattice definition of the [completed nonholomorphic Eisenstein series](../../../../../../completed-nonholomorphic-eisenstein-series.md) in Question 6 is [modular invariant](../../../../../../modular-invariant-function.md). Its [Poisson summation](../../../../../../poisson-summation-formula.md) calculation, proved there, gives the finite Laurent coefficient at $s=1$ as

$$
C(\tau)=\frac{\gamma_E-\log(4\pi)}2-\frac12\log y+\frac{\pi y}{6}-2\sum_{n\geq1}\log|1-q^n|,\qquad y=\Im\tau.
$$

The residue is constant, so $C$ is also invariant. This calculation uses only convergent Gaussian integrals and the analytic infinite product, not modularity of that product. Using the [Wirtinger derivative](../../../../../../wirtinger-derivatives.md) $\partial_\tau$, with $\partial_\tau y=1/(2i)$, differentiation of the locally uniformly convergent series gives

$$
\partial_\tau C=-\frac{\pi i}{12}\left(E_2(\tau)-\frac3{\pi y}\right).
$$

Differentiate $C(\gamma\tau)=C(\tau)$ to see that $E_2^*=E_2-3/(\pi y)$ transforms with weight two. Substituting $\Im(\gamma\tau)=y/|j|^2$ yields

$$
E_2(\gamma\tau)-j^2E_2(\tau)=\frac3{\pi y}(|j|^2-j^2)
=\frac{12c}{2\pi i}j,
$$

since $\overline j-j=-2icy$. This is the [weight-two transformation from an invariant Eisenstein limit](../../../../../../weight-two-transformation-from-an-invariant-eisenstein-limit.md).

Combine this law with the [derivative transformation of a weak modular form](../../../../../../derivative-transformation-of-a-weak-modular-form.md) proved in part (i). The anomalous terms in $Df-(k/12)E_2f$ cancel exactly, leaving the weight-$k+2$ transformation law. Both functions are holomorphic on the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md), and their [Fourier expansions](../../../../../../fourier-series-split.md) contain no negative powers. Hence the [Serre derivative](../../../../../../serre-derivative.md) satisfies

$$
\boxed{D_kf:=Df-\frac{k}{12}E_2f\in M_{k+2}.}
$$

Its constant coefficient is $-ka_0(f)/12$; it need not be a [cusp form](../../../../../../cusp-form.md) when $f$ is not cuspidal.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
