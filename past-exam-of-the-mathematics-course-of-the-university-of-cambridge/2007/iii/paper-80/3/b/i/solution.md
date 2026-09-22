<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Represent the thin layer by its [wave phase](../../../../../../../phase-waves.md) jump at the exit $x=0$ and take the incident envelope to have amplitude one. Then $E(0,z)=e^{i\phi(z)}$. [Stationarity](../../../../../../../stationary-process.md) makes the [wave phase](../../../../../../../phase-waves.md) mean a constant $\mu$; it need not be zero, since the question specifies only the [variance](../../../../../../../variance-split.md). For a [normal distribution](../../../../../../../normal-distribution.md) marginal, write $\phi=\mu+\sigma Z$ with $Z\sim N(0,1)$. If $F(t)=\mathbb E[e^{itZ}]$, integration by parts in the Gaussian density gives $F'(t)=-tF(t)$ and $F(0)=1$, hence $F(t)=e^{-t^2/2}$. Thus its [characteristic function](../../../../../../../characteristic-function.md) gives

$$
\langle E(0,z)\rangle=\langle e^{i\phi(z)}\rangle=e^{i\mu-\sigma^2/2}\equiv M.
$$

The [Fourier transform](../../../../../../../fourier-transform.md) of this constant is $2\pi M\delta(\nu)$, interpreted distributionally for the infinite [plane wave](../../../../../../../plane-wave.md). Applying the propagator from part (a),

$$
\boxed{\langle\widehat E(x,\nu)\rangle
=2\pi e^{i\mu-\sigma^2/2}\delta(\nu)e^{-i\nu^2x/(2k)}
=2\pi e^{i\mu-\sigma^2/2}\delta(\nu)}.
$$

If the [wave phase](../../../../../../../phase-waves.md) has zero mean, omit $e^{i\mu}$. A nonunit incident amplitude simply multiplies the expression. Only the one-point [Gaussian distribution](../../../../../../../normal-distribution.md) is needed for this [expected value](../../../../../../../expected-value.md); no assumption about joint [Gaussian distributions](../../../../../../../normal-distribution.md) at separated points is needed.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 80](../../../../paper-80-split.md)
5. [Iii](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
