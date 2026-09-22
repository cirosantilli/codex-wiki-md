<h1 id="17/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $I_n=\int e^{nx}\sin x\,dx$ and $J_n=\int e^{nx}\cos x\,dx$. Integrating the [trigonometric functions](../../../../../trigonometric-function.md) and differentiating $e^{nx}$ in [integration by parts](../../../../../integration-by-parts.md) gives, modulo constants,

$$
I_n=-e^{nx}\cos x+nJ_n,\qquad J_n=e^{nx}\sin x-nI_n.
$$

Substitution yields $(1+n^2)I_n=e^{nx}(n\sin x-\cos x)$ and $(1+n^2)J_n=e^{nx}(n\cos x+\sin x)$. Therefore

$$
\begin{aligned}
\int e^{nx}(\sin x-\cos x)\,dx&=I_n-J_n\\
&=\boxed{-\frac{e^{nx}}{n^2+1}\left[(1+n)\cos x+(1-n)\sin x\right]+C.}
\end{aligned}
$$

No division by $n$ was used, so this formula also applies at $n=0$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [17](../../17.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
