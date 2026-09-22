<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

Consider the [meromorphic function](../../../../../meromorphic-function.md)

$$
f(z)=\frac{e^{iz}}{z(z^2-1)}.
$$

Close the [contour](../../../../../contour-integration.md) with a large semicircle in the upper half-plane, indenting above the three real [pole](../../../../../pole.md) $-1,0,1$. The large-arc integral vanishes by [Jordan's lemma](../../../../../jordan-s-lemma.md), while the [upper-half-plane indentation rule](../../../../../upper-half-plane-indentation-rule.md) gives

$$
\operatorname{PV}\int_{-\infty}^{\infty}
\frac{e^{ix}}{x(x^2-1)}\,dx
=i\pi\sum_{a\in\{-1,0,1\}}\operatorname{Res}(f,a).
$$

The three [residue](../../../../../residue.md) are

$$
\operatorname{Res}(f,-1)=\frac{e^{-i}}2,
\qquad
\operatorname{Res}(f,0)=-1,
\qquad
\operatorname{Res}(f,1)=\frac{e^i}2.
$$

Their sum is $\cos1-1$, so the [residue theorem](../../../../../residue-theorem.md) yields

$$
\operatorname{PV}\int_{-\infty}^{\infty}
\frac{e^{ix}}{x(x^2-1)}\,dx
=i\pi(\cos1-1).
$$

The real part of the integrand is an [odd function](../../../../../odd-function.md), so its full-line principal value is zero. Its imaginary part,

$$
\frac{\sin x}{x(x^2-1)},
$$

is an [even function](../../../../../even-function.md). Taking imaginary parts and halving the full-line integral therefore gives

$$
\boxed{
\operatorname{PV}\int_0^\infty\frac{\sin x}{x(x^2-1)}\,dx
=\frac\pi2(\cos1-1)
}.
$$

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
