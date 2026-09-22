<h1 id="11h/solution">Solution</h1>

↑ **Parent:** [11H](../11h.md)

The radius of the [surface of revolution](../../../../../surface-of-revolution.md) is $|y(x)|$, so its area and the curve's [arc length](../../../../../arc-length.md) are

$$
\boxed{A[y]=2\pi\int_{-a}^{a}|y|\sqrt{1+y'^2}\,dx,\qquad
L[y]=\int_{-a}^{a}\sqrt{1+y'^2}\,dx.}
$$

For the proposed curve, $y<0$ on the interior. On this branch $A=-2\pi S$ with $S=\int y\sqrt{1+y'^2}\,dx$. Extremizing $S$ subject to $L=l$ is therefore equivalent to making the actual area stationary. Introduce a [Lagrange multiplier](../../../../../lagrange-multiplier.md) $\lambda$ and the augmented integrand $F=(y+\lambda)\sqrt{1+y'^2}$. The [Beltrami identity](../../../../../beltrami-identity.md) gives

$$
F-y'F_{y'}=\frac{y+\lambda}{\sqrt{1+y'^2}}=C.
$$

For the [fixed-length stationary surface of revolution](../../../../../fixed-length-stationary-surface-of-revolution.md), take

$$
y=\frac{\cosh(kx)-\cosh(ka)}k,\qquad
\lambda=\frac{\cosh(ka)}k,\quad C=\frac1k.
$$

Indeed $y'=\sinh(kx)$ and $\sqrt{1+y'^2}=\cosh(kx)$, so the Beltrami equation holds identically. It also follows directly that $F_y=\cosh(kx)$ and $d(F_{y'})/dx=\cosh(kx)$, verifying the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md). The endpoints vanish, and the length condition becomes

$$
\boxed{l=\frac{2\sinh(ka)}k.}
$$

For endpoint-fixed variations preserving this length, the augmented first variation is zero; subtracting the zero length variation proves that the area's first variation is zero. Its value, if desired, is $A=\pi[\sinh(2ka)-2ka]/k^2$.

To prove uniqueness, put $s=ka>0$. The equation is $\sinh s/s=l/(2a)>1$. Its derivative is $(s\cosh s-\sinh s)/s^2$. The numerator is zero at $s=0$ and has derivative $s\sinh s>0$, so the ratio increases strictly from one to infinity. The [intermediate value theorem](../../../../../intermediate-value-theorem.md) gives **exactly one positive $k$**. The stated upper bound on $l$ is not needed for this uniqueness argument. Stationarity has been proved, without making an unsupported global-minimum claim.

## ↑ Ancestors (10)

1. [11H](../11h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
