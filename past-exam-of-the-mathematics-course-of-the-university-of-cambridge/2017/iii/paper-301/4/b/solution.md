<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $H=H_0+H_{\mathrm{int}}$, the [interaction picture](../../../../../../interaction-picture.md) has $H_I(t)=e^{iH_0(t-t_0)}H_{\mathrm{int}}(t)e^{-iH_0(t-t_0)}$ and

$$
i\frac{d}{dt}|\psi(t)\rangle_I=H_I(t)|\psi(t)\rangle_I.
$$

The trial solution $|\psi(t)\rangle_I=U(t,t_0)|\psi(t_0)\rangle_I$ works for arbitrary initial states precisely when

$$
\boxed{i\partial_tU(t,t_0)=H_I(t)U(t,t_0),\qquad U(t_0,t_0)=I.}
$$

For $t\geq t_0$, the [Dyson series](../../../../../../dyson-series.md) writes

$$
U(t,t_0)=T\exp\!\left(-i\int_{t_0}^tH_I(s)ds\right)
=I+\sum_{n\geq1}(-i)^n\int_{t_0}^t ds_1\int_{t_0}^{s_1}ds_2\cdots\int_{t_0}^{s_{n-1}}ds_n\,H_I(s_1)\cdots H_I(s_n).
$$

It is also $\sum_{n\geq0}(-i)^n/n!\int_{[t_0,t]^n}d^ns\,T\{H_I(s_1)\cdots H_I(s_n)\}$: the cube consists of $n!$ ordered simplexes with the same time-ordered integrand. Differentiating the nested integrals makes the latest operator $H_I(t)$ the leftmost factor, leaving the $(n-1)$-fold integral. Thus $\partial_tU=-iH_I(t)U$ and at $t=t_0$ every nonconstant term vanishes. This proves the [differentiation of the Dyson time-ordered exponential](../../../../../../differentiation-of-the-dyson-time-ordered-exponential.md) identity without incorrectly treating the generally noncommuting Hamiltonians as [scalars](../../../../../../scalar.md).

For a Hermitian [Hamiltonian operator](../../../../../../hamiltonian-quantum-mechanics.md), $\partial_t(U^\dagger U)=iU^\dagger H_IU-iU^\dagger H_IU=0$, so the initial condition makes $U$ a [unitary operator](../../../../../../unitary-operator.md). Evolution backwards in time is its inverse, with anti-time ordering. For bounded norm-continuous $H_I$ the series converges in operator norm and the differentiation is justified by the factorial estimates. In [quantum field theory](../../../../../../quantum-field-theory-split.md), unbounded operators and products of fields require domain or regulator assumptions; this computation is the formal perturbative identity unless those analytic assumptions are supplied.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 301](../../../paper-301-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
