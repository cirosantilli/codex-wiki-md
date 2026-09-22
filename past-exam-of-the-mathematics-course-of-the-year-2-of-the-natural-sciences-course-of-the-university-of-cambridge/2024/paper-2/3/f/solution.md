<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The outward normal of the exterior region points **into the excluded disc**, so it is $-\mathbf r$ on the unit circle. Differentiating the [Dirichlet Green function](../../../../../dirichlet-green-function.md) from (e), and writing $s=|\mathbf r'|$ and $d=|\mathbf r-\mathbf r'|$, gives

$$
\begin{aligned}
\frac{\partial G}{\partial n}
&=\frac1{2\pi}\left[-\frac{1-\mathbf r\cdot\mathbf r'}{d^2}+\frac{1-\mathbf r\cdot\mathbf p}{|\mathbf r-\mathbf p|^2}\right]\\
&=\frac{s^2-1}{2\pi|\mathbf r-\mathbf r'|^2}.
\end{aligned}
$$

Here $|\mathbf r-\mathbf p|^2=d^2/s^2$ was used. The concentrated boundary data have unit integral, so the boundary representation evaluates this exterior [Poisson kernel](../../../../../poisson-kernel.md) at $\mathbf r=(-1,0)$. Thus the bounded solution on either part of the exterior $x$-axis is

$$
\boxed{\Phi(x',0)=\frac{x'^2-1}{2\pi(x'+1)^2}=\frac{x'-1}{2\pi(x'+1)},\qquad |x'|>1.}
$$

It is positive on both intervals, diverges as $x'\to-1^-$ at the boundary source, and tends to $1/(2\pi)$ as $|x'|\to\infty$. Boundedness at infinity selects this solution; otherwise one could add an arbitrary multiple of $\log|\mathbf r'|$ without changing the circle's boundary data.

## ↑ Ancestors (13)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
