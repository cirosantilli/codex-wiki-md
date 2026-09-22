<h1 id="15d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take the wire at $(a,0)$ to carry $+\lambda$ and that at $(-a,0)$ to carry $-\lambda$. If

$$
r_+=\sqrt{(x-a)^2+y^2},
\qquad
r_-=\sqrt{(x+a)^2+y^2},
$$

then, up to one additive constant,

$$
\phi=\frac{\lambda}{2\pi\varepsilon_0}
\log\frac{r_-}{r_+}.
$$

Thus an [equipotential](../../../../../../equipotential.md) with $k=2\pi\varepsilon_0\phi/\lambda$ satisfies $r_-/r_+=e^k$. For $k\ne0$, completing the square gives the [Apollonius circle](../../../../../../circles-of-apollonius.md)

$$
\boxed{
\left(x-a\coth k\right)^2+y^2
=a^2\operatorname{csch}^2k}.
$$

Its centre is $(a\coth k,0)$ and its radius is $a/|\sinh k|$. Positive and negative values give nested circles around the positive and negative wires. The electric field is orthogonal to these circles and points from the positive wire toward the negative wire. For $\phi=0$, the limiting equipotential is the straight line $x=0$.

Direct superposition gives

$$
\mathbf E
=\frac{\lambda}{2\pi\varepsilon_0}
\left[
\frac{(x-a,y)}{(x-a)^2+y^2}
-\frac{(x+a,y)}{(x+a)^2+y^2}
\right].
$$

In the limit $a\to0$ with $\lambda a=p$, the potential and field become those of a two-dimensional [electric dipole](../../../../../../electric-dipole.md):

$$
\boxed{\phi\longrightarrow
\frac{p}{\pi\varepsilon_0}\frac{x}{x^2+y^2}},
$$

and

$$
\boxed{
\mathbf E\longrightarrow
\frac{p}{\pi\varepsilon_0(x^2+y^2)^2}
\bigl(x^2-y^2,\,2xy\bigr)}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [15D](../../15d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
