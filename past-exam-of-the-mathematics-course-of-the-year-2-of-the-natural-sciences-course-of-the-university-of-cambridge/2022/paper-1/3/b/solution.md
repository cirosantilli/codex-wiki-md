<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose the [causal Green function](../../../../../causal-green-function.md) convention $L_xG(x,\xi)=\delta(x-\xi)$ for each source point $\xi>0$, with $G(x,\xi)=0$ when $x<\xi$. This automatically gives the two zero-origin limits. The kernel is continuous at $x=\xi$, and integrating its equation across the source requires the unit [derivative](../../../../../derivative.md) jump $\partial_xG(\xi^+,\xi)-\partial_xG(\xi^-,\xi)=1$.

For $x>\xi$, the homogeneous basis from part (a) gives a continuous kernel proportional to $x^r\log(x/\xi)$. Its derivative at $x=\xi$ is $\xi^{r-1}$, so the normalization is $\xi^{1-r}$. Hence the [causal Green function for a repeated-root Euler operator](../../../../../causal-green-function-for-a-repeated-root-euler-operator.md) is

$$
\boxed{G(x,\xi)=\begin{cases}x^r\xi^{1-r}\log(x/\xi),&x\geq\xi,\\0,&0\leq x<\xi,\end{cases}\qquad r=\frac{1-\alpha}{2},\quad\xi>0.}
$$

The same formula follows from $[y_1(\xi)y_2(x)-y_2(\xi)y_1(x)]/W(\xi)$ on the right of the source, with $W(\xi)=\xi^{-\alpha}$.

The singular endpoint matters for uniqueness. If $\alpha<-1$, then $r>1$, and both $x^r$ and $x^r\log x$, together with their first [derivatives](../../../../../derivative.md), vanish at zero. Adding any source-dependent linear combination of these homogeneous solutions to $G$ preserves the two stated origin conditions. Thus those conditions alone do not determine a unique [Green's function](../../../../../green-s-function-split.md) in that parameter range. The causal requirement used here selects the displayed kernel. For $\alpha\geq-1$ no nonzero homogeneous solution satisfies both zero-origin limits, so this ambiguity is absent.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
