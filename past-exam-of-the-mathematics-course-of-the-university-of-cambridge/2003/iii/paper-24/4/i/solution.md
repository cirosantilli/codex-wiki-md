<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [Fourier transform](../../../../../../fourier-transform.md) convention $\widehat h(\xi)=\int_{\mathbb R}h(x)e^{-2\pi ix\xi}\,dx$. For a [Schwartz function](../../../../../../schwartz-function.md) $h$, the [Poisson summation formula](../../../../../../poisson-summation-formula.md) is

$$
\boxed{\sum_{n\in\mathbb Z}h(n)=\sum_{m\in\mathbb Z}\widehat h(m).}
$$

To prove it, periodize $h$ as $P(x)=\sum_{n\in\mathbb Z}h(x+n)$. Rapid decay of all derivatives makes this a smooth periodic function, with uniform termwise differentiability. Its $m$th [Fourier coefficient](../../../../../../fourier-coefficient.md) is

$$
\int_0^1P(x)e^{-2\pi imx}\,dx=\int_{\mathbb R}h(u)e^{-2\pi imu}\,du=\widehat h(m),
$$

where [absolute convergence](../../../../../../absolute-convergence.md) justifies splitting the real-line integral into unit intervals. Integration by parts gives rapid decay of the coefficients of $P$, so its [Fourier series](../../../../../../fourier-series-split.md) converges absolutely and uniformly to $P$. Evaluate it at zero to obtain the formula.

For $\operatorname{Im}\tau>0$ and $z\in\mathbb C$, take the complex [Gaussian function](../../../../../../gaussian-function.md) $h(x)=e^{\pi i\tau x^2+2\pi izx}$. It is a Schwartz function of the real variable $x$. Its Fourier transform is

$$
\widehat h(\xi)=(-i\tau)^{-1/2}\exp\!\left(-\frac{\pi i(z-\xi)^2}{\tau}\right).
$$

The real Gaussian integral proves this first for $\tau=iy$, $y>0$, and real $z$. Normal convergence of the defining integrals makes both sides entire in $z$ and holomorphic in $\tau\in\mathbb H$, so the identity theorem extends it to the stated domain. Choose the square-root branch holomorphic for $-i\tau$ in the right half-plane and positive when $\tau=iy$.

Applying [Poisson summation](../../../../../../poisson-summation-formula.md) gives the transformation of the [Jacobi theta function](../../../../../../jacobi-theta-function.md):

$$
\vartheta_{00}(z,\tau)=(-i\tau)^{-1/2}e^{-\pi iz^2/\tau}\sum_{m\in\mathbb Z}e^{-\pi im^2/\tau+2\pi imz/\tau}.
$$

The series on the right is $\vartheta_{00}(z/\tau,-1/\tau)$. Rearranging therefore gives

$$
\boxed{\vartheta_{00}(z/\tau,-1/\tau)=\left(\frac\tau i\right)^{1/2}e^{\pi iz^2/\tau}\vartheta_{00}(z,\tau).}
$$

The branch choice is part of the formula; at $\tau=i$ its square-root factor equals one.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
