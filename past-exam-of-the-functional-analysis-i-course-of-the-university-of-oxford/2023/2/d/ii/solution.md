<h1 id="2/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

When $p=\infty$, $p'=1$ and $T_hf=h^{-1}\int_{-h}^h f(x)\,dx$. Take the bounded [measurable function](../../../../../measurable-function.md)

$$
f(x)=\begin{cases}\sin(\log|x|),&x\ne0,\\0,&x=0.\end{cases}
$$

It represents an element of the [Lp space](../../../../../lp-space.md) $L^\infty((-1,1))$, with [L-infinity norm](../../../../../l-infinity-norm.md) at most one. Since

$$
\int_0^h\sin(\log x)\,dx
=\frac h2\bigl(\sin(\log h)-\cos(\log h)\bigr),
$$

where the lower endpoint contributes zero, its symmetric [Lebesgue integral](../../../../../lebesgue-integral.md) gives

$$
T_hf=\sin(\log h)-\cos(\log h).
$$

For $h_n=e^{-2\pi n}$ and $\widetilde h_n=e^{-(2\pi n+\pi)}$, both [sequences](../../../../../sequence.md) tend to zero through $(0,1)$, but $T_{h_n}f=-1$ and $T_{\widetilde h_n}f=1$. Therefore

$$
\boxed{f\notin Y,\qquad Y\subsetneq L^\infty((-1,1)).}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analysis I course of the University of Oxford](../../../../split.md)
6. [Functional analysis I course of the University of Oxford](../../../../../functional-analysis-i-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
