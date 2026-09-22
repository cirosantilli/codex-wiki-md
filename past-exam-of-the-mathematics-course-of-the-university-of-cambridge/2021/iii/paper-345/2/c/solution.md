<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The shallow-water equations cease to apply inside the narrow nose, so a [gravity-current front condition](../../../../../../gravity-current-front-condition.md) is needed to relate its speed to the depth immediately behind it. Use

$$
\boxed{\dot R=Fr\sqrt{g'h}=Fr\,c},
$$

where $Fr$ is the front [Froude number](../../../../../../froude-number.md); the ideal deep-ambient von Kármán condition gives $Fr=\sqrt2$.

In a uniform axisymmetric box model, conservation of contaminated volume gives

$$
h=\frac{V}{\pi R^2}.
$$

The total nondimensional heat content is $V\theta$, while cooling acts over area $\pi R^2$, so

$$
\boxed{
\dot\theta=-\frac{K\pi R^2}{V}\theta,
\qquad
\dot R=\frac{Fr}{R}
\sqrt{\frac{g'_0V}{\pi}}\,\theta
}.
$$

Eliminating time and taking the initial release radius as negligible gives

$$
\theta(R)=1-\frac{K\pi R^4}
{4Fr\,V\sqrt{g'_0V/\pi}}.
$$

Spreading stops as $\theta\to0$, at

$$
R_{\max}^4
=\frac{4Fr\,V}{K\pi}
\sqrt{\frac{g'_0V}{\pi}}.
$$

Hence the maximum covered area is

$$
\boxed{
A_{\max}=\pi R_{\max}^2
=2\pi
\left[
\frac{Fr\,V}{K\pi}
\sqrt{\frac{g'_0V}{\pi}}
\right]^{1/2}
}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
