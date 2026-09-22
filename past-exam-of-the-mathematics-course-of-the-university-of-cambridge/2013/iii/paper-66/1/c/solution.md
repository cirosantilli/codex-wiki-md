<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose real [eigenfunctions](../../../../../../eigenfunction.md) with $\int_0^L W_nW_m\,dx=\delta_{nm}$. For positive modes, [self-adjointness](../../../../../../self-adjoint-operator.md) and [integration by parts](../../../../../../integration-by-parts.md) diagonalize the energy:

$$
\mathcal E=\frac12\sum_n\mu_na_n^2,\qquad \mu_n=A k_n^4.
$$

At [temperature](../../../../../../temperature.md) $T$, the [canonical ensemble](../../../../../../canonical-ensemble.md) is a product of centered [Gaussian distributions](../../../../../../normal-distribution.md). The [equipartition theorem](../../../../../../equipartition-theorem.md), with [Boltzmann constant](../../../../../../boltzmann-constant.md) $k_B$, gives

$$
\langle a_n\rangle=0,\qquad\langle a_na_m\rangle=\frac{k_BT}{\mu_n}\delta_{nm}.
$$

The resulting [thermal covariance of an elastic filament](../../../../../../thermal-covariance-of-an-elastic-filament.md) is

$$
\boxed{\operatorname{Cov}(h(x),h(y))=\frac{k_BT}{A}\sum_{n:\,k_n>0}\frac{W_n(x)W_n(y)}{k_n^4},\qquad
\operatorname{Var}(h(x))=\frac{k_BT}{A}\sum_{n:\,k_n>0}\frac{W_n(x)^2}{k_n^4}.}
$$

For an unnormalized [eigenfunction](../../../../../../eigenfunction.md) of squared [L2 norm](../../../../../../l2-norm.md) $N_n$, divide its summand by $N_n$. This normalization factor cannot be absorbed silently into the modal [variance](../../../../../../variance-split.md).

For [clamped boundary conditions](../../../../../../clamped-boundary-condition.md) at both ends, the inverse of $d^4/dx^4$ has [Green function](../../../../../../green-s-function.md), for $x\leq y$,

$$
G(x,y)=\frac{x^2(L-y)^2}{6L^3}[3Ly-(L+2y)x],\qquad G(x,y)=G(y,x)\ \text{for }x\geq y.
$$

It is cubic on each side of $y$, satisfies the four clamped conditions, has continuous first two derivatives, and has unit jump in its third derivative. Thus $\partial_x^4G=\delta(x-y)$, and its [eigenfunction expansion](../../../../../../eigenfunction-expansion.md) is the sum above. In particular,

$$
\boxed{\operatorname{Var}(h(x))=\frac{k_BT}{3A L^3}x^3(L-x)^3,\qquad
\operatorname{Var}(h(L/2))=\frac{k_BT L^3}{192A}.}
$$

These finite [variances](../../../../../../variance-split.md) require removal of every [zero-energy filament mode](../../../../../../zero-energy-filament-mode.md). An unconstrained free-free [elastic filament](../../../../../../elastic-filament.md) can translate and tilt at no energy cost; a torqued-torqued [elastic filament](../../../../../../elastic-filament.md) can translate. Their unrestricted [Boltzmann distributions](../../../../../../boltzmann-distribution.md) are not normalizable, so the full displacement [variance](../../../../../../variance-split.md) is undefined. Fix those rigid degrees of freedom before applying the positive-mode formula.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
