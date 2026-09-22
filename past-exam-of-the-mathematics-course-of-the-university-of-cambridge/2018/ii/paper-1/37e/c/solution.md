<h1 id="37e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The $x$ [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) has the first integral

$$
e^{2Ht}\dot x=v_0,
$$

where the constant follows from the initial data. Combining this with [proper-time normalization](../../../../../../proper-time-normalization.md) gives the [Timelike geodesic in the expanding flat slicing of de Sitter spacetime](../../../../../../timelike-geodesic-in-the-expanding-flat-slicing-of-de-sitter-spacetime.md):

$$
-\dot t^2+e^{2Ht}\dot x^2=-1
\quad\Longrightarrow\quad
\dot t=\sqrt{1+v_0^2e^{-2Ht}}.
$$

Consequently

$$
\frac{d\tau}{dt}=\frac1{\sqrt{1+v_0^2e^{-2Ht}}}.
$$

Integrating from $t=0$, where $\tau=0$, gives

$$
\boxed{\tau(t)=\frac1{2H}\log\left[
\frac{\sqrt{1+v_0^2e^{-2Ht}}+1}
{\sqrt{1+v_0^2e^{-2Ht}}-1}
\frac{\sqrt{1+v_0^2}-1}
{\sqrt{1+v_0^2}+1}
\right].}
$$

As $t\to-\infty$, the first ratio tends to $1$, so

$$
\boxed{\tau\longrightarrow\tau_-
=-\frac1{2H}\log\frac{\sqrt{1+v_0^2}+1}
{\sqrt{1+v_0^2}-1}>-\infty.}
$$

Thus $t$ tends to $-\infty$ at the finite proper time $\tau_-$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [37E](../../37e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
