<h1 id="7b/solution">Solution</h1>

↑ **Parent:** [7B](../7b.md)

Integration by parts is legitimate after symmetrically excluding a neighborhood of zero; the boundary terms vanish because $\cos(nx)-\cos(mx)=O(x^2)$ at zero and is bounded at infinity. Hence

$$
\operatorname{PV}\int_{-\infty}^{\infty}
\frac{\cos nx-\cos mx}{x^2} dx
=-n\operatorname{PV}\int_{-\infty}^{\infty}\frac{\sin nx}{x} dx
+m\operatorname{PV}\int_{-\infty}^{\infty}\frac{\sin mx}{x} dx.
$$

The standard [Dirichlet integral](../../../../../dirichlet-integral.md), obtained by closing the contour for $e^{iaz}/z$ in the upper half-plane and indenting above its pole at zero, is

$$
\operatorname{PV}\int_{-\infty}^{\infty}\frac{\sin(ax)}x dx=\pi
\qquad(a>0).
$$

Therefore

$$
\boxed{\operatorname{PV}\int_{-\infty}^{\infty}
\frac{\cos nx-\cos mx}{x^2} dx=\pi(m-n).}
$$

## ↑ Ancestors (10)

1. [7B](../7b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
