<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**Conditioning on the observed time.** The native PDF defines $\tau_2$ as the first production time and then conditions on that production occurring at $\tau_2$. If the intended information is its numerical value $\tau_2=t$, the answer depends on $t$. We first compute this [conditional probability](../../../../conditional-probability.md) using a [conditional probability density](../../../../conditional-density.md); conditioning on an exact value of a continuous [random variable](../../../../random-variable-split.md) means a density ratio, since $\mathbb P(\tau_2=t)=0$.

Before $\tau_2$, no molecules of the second [chemical species](../../../../chemical-species.md) are present, so the joint-removal [chemical reaction](../../../../chemical-reaction-split.md) cannot occur. Molecules of the first [chemical species](../../../../chemical-species.md) arrive as a rate-$2$ [Poisson process](../../../../poisson-process-split.md), and each independently starts a clock with a rate-$1/2$ [exponential distribution](../../../../exponential-distribution.md) for producing the first molecule of the second [chemical species](../../../../chemical-species.md). Define the unnormalized [probability mass function](../../../../probability-mass-function.md)

$$
q_n(t)=\mathbb P\bigl(A_1(t)=n,\ \tau_2>t\bigr),\qquad
F(z,t)=\sum_{n=0}^\infty q_n(t)z^n.
$$

The [chemical master equation](../../../../chemical-master-equation.md) before the first production, with production treated as killing, is

$$
q_n'=2q_{n-1}-\left(2+\frac n2\right)q_n,
\qquad q_n(0)=\mathbf1_{\{n=0\}}.
$$

Multiplying by $z^n$ and summing gives a [partial differential equation](../../../../partial-differential-equation-split.md) for the [probability generating function](../../../../probability-generating-function.md):

$$
F_t=2(z-1)F-\frac z2F_z,\qquad F(z,0)=1.
$$

Its solution, verifiable by direct [differentiation](../../../../differentiation.md), is

$$
F(z,t)=\exp\bigl[-2t+m(t)z\bigr],
\qquad m(t)=4(1-e^{-t/2}).
$$

Thus $q_n(t)=e^{-2t}m(t)^n/n!$, the [survival function](../../../../survival-function.md) is $S(t)=F(1,t)=e^{-2t+m(t)}$, and the [conditional distribution](../../../../conditional-distribution.md) of $A_1(t)$ given survival to $t$ is a [Poisson distribution](../../../../poisson-distribution.md) of [mean](../../../../expected-value-split.md) $m(t)$.

Production in $(t,t+dt)$ from [Markov chain state](../../../../markov-chain-state.md) $n$ has joint [probability](../../../../probability.md) $(n/2)q_n(t)\,dt+o(dt)$. Therefore the [probability density function](../../../../probability-density-function.md) of $\tau_2$ is

$$
f_{\tau_2}(t)=\frac12\sum_{n\geq1}nq_n(t)
=\frac12m(t)S(t),\qquad t>0.
$$

The first production leaves $A_1$ unchanged. Taking the density ratio gives a [size-biased distribution](../../../../size-biased-distribution.md) of the surviving count:

$$
\mathbb P\bigl(A_1(\tau_2)=n\mid\tau_2=t\bigr)
=\frac{nq_n(t)}{m(t)S(t)}
=e^{-m(t)}\frac{m(t)^{n-1}}{(n-1)!},\qquad n\geq1.
$$

In particular, under this reading the requested [conditional probability](../../../../conditional-probability.md) is

$$
\boxed{\mathbb P\bigl(A_1(\tau_2)=2\mid\tau_2=t\bigr)
=4(1-e^{-t/2})\exp\!\bigl[-4(1-e^{-t/2})\bigr],\quad t>0.}
$$

The shift by one matters: an observation made exactly when production occurs preferentially selects larger counts, since their production [reaction propensity function](../../../../reaction-propensity-function.md) is larger.

**Without observing the numerical time.** If the conditioning merely repeats the definition of $\tau_2$, the requested [probability](../../../../probability.md) is instead the unconditional count at that [stopping time](../../../../stopping-time.md). Before production, $A_1$ increases by one at rate $2$, while production occurs at rate $n/2$ in [Markov chain state](../../../../markov-chain-state.md) $n$. The [competing exponential clocks](../../../../competing-exponential-clocks.md) imply

$$
\mathbb P\bigl(A_1(\tau_2)=2\bigr)
=\frac{2}{2+1/2}\frac{1}{2+1}
=\boxed{\frac4{15}}.
$$

The first factor requires a second arrival before production from count one; the second requires production before a third arrival. The first arrival itself is certain. Production eventually occurs with [probability](../../../../probability.md) one, as is also clear from $S(t)\to0$. As a consistency check, averaging the time-conditioned answer against $f_{\tau_2}$ gives

$$
\int_0^\infty m(t)e^{-m(t)}\frac{m(t)}2e^{-2t+m(t)}\,dt
=8\int_0^\infty e^{-2t}(1-e^{-t/2})^2\,dt
=\frac4{15}.
$$

These are two distinct, explicitly specified interpretations of the printed conditioning.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the stochastic modelling of biological processes course of the University of Oxford](../../../split.md)
5. [Stochastic modelling of biological processes course of the University of Oxford](../../../../stochastic-modelling-of-biological-processes-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
