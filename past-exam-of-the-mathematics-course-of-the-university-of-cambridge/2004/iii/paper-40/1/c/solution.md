<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Center the five coefficients at lags $-2,-1,0,1,2$. Their transfer function is real:

$$
H(\omega)=\frac{-e^{-2i\omega}+2e^{-i\omega}+4+2e^{i\omega}-e^{2i\omega}}6
=\frac{4+4\cos\omega-2\cos(2\omega)}6.
$$

Choosing consecutive causal lags instead only adds a phase and leaves the squared modulus unchanged. After $k$ applications, the [white noise](../../../../../../white-noise.md) [spectral density](../../../../../../spectral-density-of-a-stationary-process.md) has become

$$
\boxed{f_k(\omega)=\frac{\sigma^2}{2\pi}|H(\omega)|^{2k}.}
$$

Write $c=\cos\omega$. Completing the square gives

$$
H(\omega)=1+\frac23c-\frac23c^2
=\frac76-\frac23(c-\tfrac12)^2.
$$

For $-1\leq c\leq1$, its range is $[-1/3,7/6]$, and its absolute maximum is $7/6$, attained exactly when $c=1/2$. Consequently, on the conventional nonnegative frequency range $[0,\pi]$,

$$
\boxed{\frac{f_k(\omega)}{f_k(\pi/3)}
=\left(\frac{|H(\omega)|}{7/6}\right)^{2k}\longrightarrow0
\quad\text{for }\omega\ne\pi/3.}
$$

On the two-sided range $[-\pi,\pi]$ there is also a peak at $-\pi/3$; the ratio there is one for every $k$. This is a counterexample to the claim if read literally on a signed frequency domain. The correct two-sided exclusion is $\omega\ne\pm\pi/3$.

The result illustrates how [repeated symmetric filtering can amplify an oscillation](../../../../../../repeated-symmetric-filtering-can-amplify-an-oscillation.md). Although $H(0)=1$ preserves a constant component, $H(\pi/3)=7/6>1$ amplifies period-six oscillations. Repetition selects an increasingly narrow frequency band around those peaks; it does not simply smooth all noise away. In fact the unnormalized output [variance](../../../../../../variance-split.md) eventually grows without bound, since a fixed interval around either peak has $|H|>1$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
