<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose $N$ near the least term, so $\gamma=N+2/3=R+O(1)$ with $R=|z|^3$. On writing $\beta=3(\arg z-\pi/3)$, the parameter is $\lambda=Re^{i\beta}$. For $\beta=O(R^{-1/2})$,

$$
\lambda=R+iR\beta+O(1)=\gamma+i\mu\sqrt\gamma+O(1),\qquad \mu\sim\beta\sqrt R.
$$

The supplied [Gaussian pole transition for a large gamma parameter](../../../../../../gaussian-pole-transition-for-a-large-gamma-parameter.md) therefore gives $I\sim i\pi[1+\operatorname{erf}(\mu/\sqrt2)]$. Substitution in [solution](../a/solution.md) gives the smoothing formula in [solution](../solution.md) once the amplitude identity in [solution](../c/solution.md) is used.

The origin of the [error function](../../../../../../error-function.md) can also be seen locally. Set $t=1+s/\sqrt\gamma$ in the Borel integral. Then

$$
(\gamma-1)\log t+\lambda(1-t)=-\frac{s^2}{2}-i\mu s+O(\gamma^{-1/2}),\qquad \frac{dt}{1-t}=-\frac{ds}{s}.
$$

The saddle has become a [Gaussian integral](../../../../../../gaussian-integral.md) meeting a simple pole. With the upper-pole contour, the leading integral is $-\int_{\mathcal C_+}e^{-s^2/2-i\mu s}ds/s$. Its value at $\mu=0$ is $i\pi$ from the indentation. Differentiating with respect to $\mu$ gives $i\sqrt{2\pi}e^{-\mu^2/2}$, so integration from zero gives $i\pi[1+\operatorname{erf}(\mu/\sqrt2)]$. This independently fixes the sign and the half-jump on the [Stokes line](../../../../../../stokes-line.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

## ← Incoming links (1)

- [Solution](../solution.md)
