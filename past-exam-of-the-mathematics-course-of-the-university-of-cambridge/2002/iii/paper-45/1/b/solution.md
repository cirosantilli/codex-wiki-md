<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use $c=1$ and signature $+---$. The positively curved [FLRW metric](../../../../../../friedmann-lemaitre-robertson-walker-metric.md) in the usual radial chart is

$$
ds^2=dt^2-a^2(t)\left[\frac{dr^2}{1-r^2}+r^2(d\Theta^2+\sin^2\Theta\,d\phi^2)\right].
$$

Set $r=\sin\chi$ and introduce [conformal time](../../../../../../conformal-time.md) by $dt=a\,d\eta$. Then $dr^2/(1-r^2)=d\chi^2$ in the chart, and the spherical polar coordinate $\chi\in[0,\pi]$ extends the spatial description to the full [three-sphere](../../../../../../three-sphere.md). Thus

$$
\boxed{ds^2=a^2(\eta)\left[d\eta^2-d\chi^2-\sin^2\chi(d\Theta^2+\sin^2\Theta\,d\phi^2)\right].}
$$

The $r$ coordinate itself is not one-to-one across the equator, which is why the new polar coordinate is useful.

For $\Lambda=0$ and $k=1$, the [Friedmann equation](../../../../../../friedmann-equations.md) is $\dot a^2=(8\pi G/3)\rho a^2-1$. Since $a'=a\dot a$, it becomes

$$
\boxed{(a')^2=\frac{8\pi G\rho}{3}a^4-a^2.}
$$

For [pressureless matter](../../../../../../pressureless-matter.md), the background [continuity equation](../../../../../../continuity-equation.md) gives $\rho a^3=\rho_0a_0^3$. Define the conserved normalization $M=(4\pi/3)\rho_0a_0^3$. It makes the equation $(a')^2=2GMa-a^2$. The [closed matter-dominated Friedmann solution](../../../../../../closed-matter-dominated-friedmann-solution.md) is the cycloid

$$
\boxed{a(\eta)=GM(1-\cos\eta),\qquad t(\eta)=GM(\eta-\sin\eta).}
$$

Indeed $a'=GM\sin\eta$ and $2GMa-a^2=(GM)^2\sin^2\eta$. Integrating $dt/d\eta=a$ gives the second expression, with the [Big Bang](../../../../../../big-bang.md) at $t=\eta=0$. It expands to $a=2GM$ at $\eta=\pi$ and recollapses at $\eta=2\pi$. Here $M$ is the constant appearing in the Friedmann equation; it is not the total mass of the entire closed spatial slice, whose volume is $2\pi^2a^3$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
