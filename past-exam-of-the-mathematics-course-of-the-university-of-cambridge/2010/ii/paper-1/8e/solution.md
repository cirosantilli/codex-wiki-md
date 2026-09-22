<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

The real part of a [holomorphic function](../../../../../holomorphic-function.md) is real analytic and has a local complexification in its two real coordinates. Define $f^*(w)=\overline{f(\bar w)}$. On real $(x,y)$,

$$
2u(x,y)=f(x+iy)+f^*(x-iy),
$$

and the same identity holds after analytic continuation to complex $(x,y)$. Substituting $x=(z+\bar z_0)/2$ and $y=(z-\bar z_0)/(2i)$ gives $x+iy=z$ and $x-iy=\bar z_0$, hence

$$
\boxed{f(z)=2u\left(\frac{z+\bar z_0}{2},\frac{z-\bar z_0}{2i}\right)-\overline{f(z_0)}.}
$$

The conjugation on the final constant is present in the PDF but was lost in the converted TeX. Without it the formula already fails when $z=z_0$ and $f(z_0)$ is not real.

Now $ze^{iz}=(x+iy)e^{-y}(\cos x+i\sin x)$ has the specified real part. Thus the complete family is

$$
\boxed{f(z)=ze^{iz}+iC,\qquad C\in\mathbb R.}
$$

Any two such [holomorphic functions](../../../../../holomorphic-function.md) differ by a [holomorphic function](../../../../../holomorphic-function.md) with zero real part; the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) make its imaginary part constant on a connected neighborhood.

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
