<h1 id="14e/solution">Solution</h1>

↑ **Parent:** [14E](../14e.md)

Choose $\log u$ with $-\pi<\arg u<\pi$. The cut's upper and lower banks have $u=-x$, $x\in(0,1)$, and give

$$
i(-e^{i\pi z}+e^{-i\pi z})\int_0^1\frac{x^{z-1}}{x^2+4x+1}\,dx
=2\sin(\pi z)\int_0^1\frac{x^{z-1}}{x^2+4x+1}\,dx.
$$

The small circle about zero vanishes for $\operatorname{Re}z>0$. On the unit circle put $u=e^{i\theta}$. Since $u^2-4u+1=-2u(2-\cos\theta)$, its contribution is

$$
G(z)=\frac12\int_{-\pi}^{\pi}\frac{e^{i(z-1)\theta}}{2-\cos\theta}\,d\theta.
$$

Using $2-\cos\theta=1+2\sin^2(\theta/2)$ gives the required decomposition.

The only enclosed [pole](../../../../../pole.md) is $a=2-\sqrt3$; the other root $2+\sqrt3$ is outside. The [residue theorem](../../../../../residue-theorem.md), including the factor $i$ in front of the contour integral, gives

$$
\boxed{I(z)=i(2\pi i)\frac{a^{z-1}}{2a-4}=\frac{\pi}{\sqrt3}(2-\sqrt3)^{z-1}}.
$$

Here the positive real logarithm defines the power, so this expression is an [entire function](../../../../../entire-function.md) of $z$. The finite-interval integral $G$ is also entire, by differentiation under the integral on compact sets. Therefore **$F(z)=\frac{\pi}{\sqrt3}(2-\sqrt3)^{z-1}-G(z)$** is an [analytic continuation](../../../../../analytic-continuation.md) valid on the whole complex plane. Outside $\operatorname{Re}z>0$ it is this continuation, rather than the unregularized cut integral, that defines $F$.

## ↑ Ancestors (10)

1. [14E](../14e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
