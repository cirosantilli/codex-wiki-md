<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $\xi=hk$. For the [discrete Fourier mode](../../../../../../discrete-fourier-mode.md), the displacement difference in the $l$th neighbor pair carries $e^{il\xi}-1$, and

$$
\sum_{l\ne0}\frac{e^{il\xi}-1}{|l|^3}=2\sum_{l=1}^\infty\frac{\cos(l\xi)-1}{l^3}=-F(\xi).
$$

Thus the infinite system reduces to

$$
\boxed{s^2X-2\Omega sY=3\Omega^2X-\frac{Gm}{h^3}F(\xi)X,\qquad s^2Y+2\Omega sX=2\frac{Gm}{h^3}F(\xi)Y.}
$$

The [gravitating lattice Fourier kernel](../../../../../../gravitating-lattice-fourier-kernel.md) $F$ is nonnegative, even and $2\pi$-periodic, with $F(0)=0$. The [uniform convergence](../../../../../../uniform-convergence.md) and [absolute convergence](../../../../../../absolute-convergence.md) of its differentiated series gives

$$
F'(\xi)=2\sum_{l=1}^\infty\frac{\sin(l\xi)}{l^2}.
$$

To prove the maximum, it is not sufficient to maximize each cosine term separately: the even terms do not reach their individual maxima at $\pi$. Instead use the convergent integral representation $l^{-2}=\int_0^\infty t e^{-lt}dt$. Summing the [geometric series](../../../../../../geometric-series.md) for sines gives

$$
F'(\xi)=2\sin\xi\int_0^\infty\frac{t e^{-t}}{1-2e^{-t}\cos\xi+e^{-2t}}\,dt.
$$

For $0<\xi<\pi$, the denominator is positive and $\sin\xi>0$, so $F'>0$. For $\pi<\xi<2\pi$, $F'<0$. The interchange is justified by $\sum_l\int_0^\infty t e^{-lt}|\sin(l\xi)|dt\le\sum_l l^{-2}<\infty$. Hence

$$
\boxed{F\text{ has its global maxima exactly at }\xi=(2j+1)\pi.}
$$

Their value is

$$
\boxed{F(\pi)=4\sum_{l\text{ odd}}l^{-3}=\frac72\zeta(3),}
$$

where $\zeta$ is the [Riemann zeta function](../../../../../../riemann-zeta-function.md). This maximizing [Fourier mode](../../../../../../fourier-mode.md) alternates the signs of neighboring particle displacements.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
