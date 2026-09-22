<h1 id="3/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $p\in\mathcal U^*$, the definition of the [convex conjugate](../../../../../../../convex-conjugate.md) gives

$$
\begin{aligned}
(E\mathbin\square F)^*(p)
&=\sup_u\sup_v\{\langle p,u\rangle-E(v)-F(u-v)\}\\
&=\sup_{v,w}\{\langle p,v\rangle-E(v)+\langle p,w\rangle-F(w)\}\\
&=E^*(p)+F^*(p),
\end{aligned}
$$

where the substitution $w=u-v$ is a bijection of the independent pairs. Therefore

$$
\boxed{(E\mathbin\square F)^*=E^*+F^*.}
$$

This [infimal convolution](../../../../../../../infimal-convolution.md) identity does not need [convexity](../../../../../../../convex-function.md) of $E,F$ or attainment of the inner [infimum](../../../../../../../infimum.md). The assumptions ensure that both functions have nonempty [effective domains](../../../../../../../effective-domain.md); their conjugates never take $-\infty$, so the separated sum is well defined, allowing $+\infty$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [3](../../../3.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
