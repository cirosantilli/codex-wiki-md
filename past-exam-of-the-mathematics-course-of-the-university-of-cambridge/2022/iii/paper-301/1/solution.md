<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a Schrödinger-picture state satisfying

$$
i\frac d{dt}|\psi(t)\rangle_S=(H_0+\lambda H_{\rm int})|\psi(t)\rangle_S,
$$

define the [interaction picture](../../../../../interaction-picture.md) by

$$
|\psi(t)\rangle_I=e^{iH_0t}|\psi(t)\rangle_S,
\qquad
O_I(t)=e^{iH_0t}O_Se^{-iH_0t}.
$$

Differentiation gives

$$
i\frac d{dt}|\psi(t)\rangle_I=H_I(t)|\psi(t)\rangle_I,
\qquad
H_I(t)=\lambda e^{iH_0t}H_{\rm int}e^{-iH_0t}.
$$

The formal solution from $t_0$ is the [Dyson series](../../../../../dyson-series.md)

$$
U_I(t,t_0)=\mathcal T\exp\!\left[-i\int_{t_0}^tH_I(s)\,ds\right].
$$

Through quadratic order,

$$
\begin{aligned}
U_I(t,t_0)
&=1-i\int_{t_0}^t dt_1H_I(t_1)\\
&\quad-\int_{t_0}^tdt_1\int_{t_0}^{t_1}dt_2H_I(t_1)H_I(t_2)+O(\lambda^3).
\end{aligned}
$$

Differentiating gives

$$
i\partial_tU_I(t,t_0)
=H_I(t)\left[1-i\int_{t_0}^tH_I(t_2)dt_2\right]+O(\lambda^3)
=H_I(t)U_I(t,t_0)+O(\lambda^3),
$$

which checks the equation to the requested order.

At the endpoints, $|i\rangle_I=e^{-iH_0T/2}|i\rangle_S$ and $|f\rangle_I=e^{iH_0T/2}|f\rangle_S$. Therefore

$$
\mathcal T={}_I\langle f|U_I(T/2,-T/2)|i\rangle_I,
$$

where

$$
U_I(T/2,-T/2)
=\mathcal T\exp\!\left[-i\lambda\int_{-T/2}^{T/2}dt\int d^3x\,
\phi_{1,I}(x)\phi_{2,I}(x)^3\right].
$$

For $\phi_1(p_1)\to\phi_2(p'_1)\phi_2(p'_2)\phi_2(p'_3)$, the leading term is

$$
\mathcal A=-i\lambda\int d^4x\,
\langle p'_1p'_2p'_3|\phi_1(x)\phi_2(x)^3|p_1\rangle.
$$

There are $3!$ contractions of the identical outgoing fields. With covariantly normalized states,

$$
\boxed{\mathcal A=-i\,3!\lambda(2\pi)^4
\delta^{(4)}(p_1-p'_1-p'_2-p'_3)}.
$$

Equivalently, the interaction vertex from $-\lambda\phi_1\phi_2^3$ is $-i3!\lambda$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 301](../../paper-301-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
