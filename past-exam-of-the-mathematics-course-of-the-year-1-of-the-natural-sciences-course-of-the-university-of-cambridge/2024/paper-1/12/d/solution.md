<h1 id="12/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [spherical coordinates](../../../../../spherical-coordinate-system.md) $(r,\theta,\phi)$ centred on the right-hand [sphere](../../../../../sphere.md), with polar axis pointing outwards along $s$. The [Jacobian determinant](../../../../../jacobian-determinant.md) is $r^2\sin\theta$, and the retained region is $r\leq R$ with $r\cos\theta\geq-d$.

For $0\leq r\leq d$, every polar [angle](../../../../../angle.md) $0\leq\theta\leq\pi$ is allowed. For $d<r\leq R$, the cut requires $0\leq\theta\leq\arccos(-d/r)$. Splitting the [volume integral](../../../../../volume-integral.md) at $r=d$ therefore gives

$$
\begin{aligned}
M_e={}&\rho\int_0^{2\pi}\left[\int_0^d\int_0^\pi r^2\sin\theta\,d\theta\,dr+\int_d^R\int_0^{\arccos(-d/r)}r^2\sin\theta\,d\theta\,dr\right]d\phi\\
={}&2\pi\rho\left[2\int_0^d r^2\,dr+\int_d^R r^2\left(1+\frac dr\right)\,dr\right]\\
={}&2\pi\rho\left[\frac{2d^3}{3}+\frac{R^3-d^3}{3}+\frac d2(R^2-d^2)\right]\\
={}&\boxed{\pi\rho\left(\frac{2R^3}{3}+R^2d-\frac{d^3}{3}\right).}
\end{aligned}
$$

Substitution of $R=\beta a$ and $d=(\alpha-\gamma)a$ reproduces the [mass](../../../../../mass.md) in part (c). The radial split avoids integrating over a polar [angle](../../../../../angle.md) range independent of $r$, which would incorrectly include part of the removed [spherical cap](../../../../../spherical-cap.md).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [12](../../12.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
