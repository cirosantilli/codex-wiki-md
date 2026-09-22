<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At the empty [Markov chain state](../../../../markov-chain-state.md), only the constant-rate production [chemical reaction](../../../../chemical-reaction-split.md) is possible. Thus the [first-passage time](../../../../first-passage-time.md) $\tau_1$ has an [exponential distribution](../../../../exponential-distribution.md) of rate $2$:

$$
\mathbb P(\tau_1>t)=e^{-2t},\qquad t\geq0.
$$

Its [expected value](../../../../expected-value-split.md) can be obtained by integrating this [survival function](../../../../survival-function.md), and its second [moment](../../../../moment.md) by integrating $2t$ times the [survival function](../../../../survival-function.md):

$$
\mathbb E\tau_1=\int_0^\infty e^{-2t}\,dt=\frac12,
\qquad
\mathbb E\tau_1^2=2\int_0^\infty te^{-2t}\,dt=\frac12.
$$

Consequently the requested [expected value](../../../../expected-value-split.md) and [variance](../../../../variance-split.md) are

$$
\boxed{\mathbb E\tau_1=\frac12,\qquad \operatorname{Var}(\tau_1)=\frac14.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
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
