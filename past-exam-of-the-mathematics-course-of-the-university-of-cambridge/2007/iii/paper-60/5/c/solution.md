<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $K=\sqrt\gamma(a\otimes dB^\dagger-a^\dagger\otimes dB)$, with the time argument suppressed. Since the incoming field commutes with the adapted cavity operators,

$$
K^2=\gamma\{a^2\otimes(dB^\dagger)^2-aa^\dagger\otimes dB^\dagger dB-a^\dagger a\otimes dB\,dB^\dagger+(a^\dagger)^2\otimes(dB)^2\}.
$$

Applying the [Gaussian quantum noise Ito table](../../../../../../gaussian-quantum-noise-ito-table.md) gives

$$
K^2=-\gamma\,dt\,Q\otimes I_B,\qquad Q=Naa^\dagger+(N+1)a^\dagger a-M(a^\dagger)^2-M^*a^2.
$$

The [power series](../../../../../../power-series.md) expansion $e^K=I+K+K^2/2+\cdots$ consequently becomes, through Ito order $dt$,

$$
\boxed{U_I=I+\sqrt\gamma(a\otimes dB^\dagger-a^\dagger\otimes dB)-\frac\gamma2Q\otimes I_B\,dt.}
$$

This has precisely the required quadratic drift correction. The short-time ordering is essential: the linear noise term is order $\sqrt{\gamma dt}$ and the drift is order $\gamma dt$; higher stochastic orders are discarded in the differential limit. A remainder written merely as a power of $\gamma$ is a formal coupling expansion, not a dimensionally complete statement of the short-time error.

As a sign check, $K^\dagger=-K$ and $Q^\dagger=Q$. Thus $U_I^\dagger U_I=I-\gamma Qdt-K^2=I$ through this order. The cross term is needed for stochastic [unitarity](../../../../../../unitary-operator.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
