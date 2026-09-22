<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Starting in state $1$, the onset waiting time has the [exponential distribution](../../../../../../exponential-distribution.md) of rate $\lambda$. Thus **the probability of onset before the next screen** is $1-e^{-\lambda t}$. This counts individuals who have already progressed to clinical disease as well as those still pre-clinical.

Conditional on onset at time $u<t$, the [Markov property](../../../../../../markov-property.md) makes the remaining progression time exponential with rate $\nu$. Thus **the probability of clinical progression before the screen**, conditional on that onset time, is $1-e^{-\nu(t-u)}$.

Integrating over the onset density gives the unconditional clinical probability

$$
P_{13}(t)=\int_0^t\lambda e^{-\lambda u}\bigl(1-e^{-\nu(t-u)}\bigr)\,du=1-\frac{\nu e^{-\lambda t}-\lambda e^{-\nu t}}{\nu-\lambda}.
$$

The probability of being pre-clinical at the next screen is instead

$$
P_{12}(t)=\int_0^t\lambda e^{-\lambda u}e^{-\nu(t-u)}\,du=\frac{\lambda}{\nu-\lambda}(e^{-\lambda t}-e^{-\nu t}).
$$

Together with $P_{11}(t)=e^{-\lambda t}$ and the [exponential distribution](../../../../../../exponential-distribution.md) for a patient initially in state $2$, **the transition matrix** is

$$
\boxed{P(t)=\begin{pmatrix}e^{-\lambda t}&\frac{\lambda(e^{-\lambda t}-e^{-\nu t})}{\nu-\lambda}&1-\frac{\nu e^{-\lambda t}-\lambda e^{-\nu t}}{\nu-\lambda}\\0&e^{-\nu t}&1-e^{-\nu t}\\0&0&1\end{pmatrix}.}
$$

This equals the [matrix exponential](../../../../../../matrix-exponential.md) $e^{Qt}$. The assumed unequal intensities avoid a zero denominator; at $\lambda=\nu$ the continuous limit is $P_{12}(t)=\lambda t e^{-\lambda t}$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
