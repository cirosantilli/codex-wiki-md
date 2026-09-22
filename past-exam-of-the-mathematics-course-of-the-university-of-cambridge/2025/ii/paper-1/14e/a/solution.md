<h1 id="14e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Hankel contour](../../../../../../hankel-contour.md) about the negative real axis: it starts at $-\infty$ below the cut, circles the origin counterclockwise, and returns to $-\infty$ above the cut. Take $-\pi<\arg t<\pi$. For $\operatorname{Re}s>0$, the small circle vanishes and the two banks give

$$
\int_{-\infty}^{(0+)}\frac{t^{s-1}}{e^t+e^{-t}}dt
=2i\sin(\pi s)\int_0^\infty\frac{x^{s-1}}{e^x+e^{-x}}dx.
$$

The [gamma reflection formula](../../../../../../gamma-reflection-formula.md) then gives

$$
\frac{\Gamma(1-s)}{2\pi i}(2i\sin\pi s)\int_0^\infty\frac{x^{s-1}}{e^x+e^{-x}}dx
=\frac1{\Gamma(s)}\int_0^\infty\frac{x^{s-1}}{e^x+e^{-x}}dx=\beta(s).
$$

Near zero,

$$
\frac1{e^t+e^{-t}}=\frac12-\frac14t^2+\frac5{48}t^4-\cdots.
$$

Subtracting any desired number of these terms makes the local contour [integral](../../../../../../integral.md) converge in successively larger left half-planes. The resulting apparent singularities are removable after multiplication by $\Gamma(1-s)$, so the Hankel formula analytically continues $\beta$ to all $s\in\mathbb C$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [14E](../../14e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
