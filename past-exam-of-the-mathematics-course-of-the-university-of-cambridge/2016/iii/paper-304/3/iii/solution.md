<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Rescale $W\mapsto tW$ with $t>0$. After [Berezin integration](../../../../../../berezin-integral.md), the unnormalized [holomorphic function](../../../../../../holomorphic-function.md) insertion is

$$
I_t[f]=\int_{\mathbb C}d^2z\,t^2|P'|^2f(z)e^{-t^2|P|^2}.
$$

Its derivative is an ordinary total derivative:

$$
\frac{dI_t[f]}{dt}=2t\int_{\mathbb C}d^2z\,fP'\overline{P'}(1-t^2|P|^2)e^{-t^2|P|^2}=2t\int_{\mathbb C}d^2z\,\partial_{\bar z}\left(fP'\overline P e^{-t^2|P|^2}\right)=0.
$$

The last equality again follows from polynomial growth and exponential decay. Thus the insertion is independent of $t$, and [supersymmetric localization](../../../../../../supersymmetric-localization.md) allows evaluation as $t\to\infty$ at the zeros of $P$, as in [localization of a zero-dimensional polynomial model](../../../../../../localization-of-a-zero-dimensional-polynomial-model.md).

For a simple zero $z_a$, $P(z)=P'(z_a)(z-z_a)+O((z-z_a)^2)$. The local [Gaussian integral](../../../../../../gaussian-integral.md) cancels the factor $|P'(z_a)|^2$ and contributes $\pi f(z_a)$. For a zero with [multiplicity of a root](../../../../../../multiplicity-of-a-root.md) $m_a$, write $P(z)=a_a(z-z_a)^{m_a}+\cdots$. Its leading radial integral is

$$
2\pi t^2m_a^2|a_a|^2\int_0^\infty \rho^{2m_a-1}e^{-t^2|a_a|^2\rho^{2m_a}}\,d\rho=\pi m_a.
$$

The insertion tends to $f(z_a)$ there; contributions away from the zeros vanish. Therefore **the full answer, including degenerate critical points**, is

$$
\boxed{\langle f(z)\rangle=\pi\sum_{a:P(z_a)=0}m_a f(z_a).}
$$

This is an unnormalized expectation. For simple zeros all $m_a=1$; division by $Z=\pi r$ would give the normalized average, but is not part of the requested insertion. Taking $f=1$ recovers the [partition function](../../../../../../canonical-partition-function.md), and taking $f=Pg$ recovers its vanishing [supersymmetric Ward identity](../../../../../../supersymmetric-ward-identity.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 304](../../../paper-304-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
