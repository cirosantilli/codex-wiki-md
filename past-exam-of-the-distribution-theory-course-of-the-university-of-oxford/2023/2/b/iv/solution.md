<h1 id="2/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $M=\sup_j j^{-m}\|g_j\|_{L^1}<\infty$. For each $j$, apply the [periodic primitives with zero mean](../../../../../periodic-primitive-with-zero-mean.md) construction of part (iii) to $g_j$, writing $h_{j,0}=g_j$ and

$$
h_{j,r+1}=Rh_{j,r}-\int_0^1Rh_{j,r}.
$$

The estimates are independent of $j$: $\|h_{j,r}\|_{L^1}\leq\|g_j\|_{L^1}$. With $N=m+1$, the same repeated [integration by parts](../../../../../integration-by-parts.md) gives, for every [test function](../../../../../test-function.md) $\phi\in\mathcal D(0,1)$,

$$
\begin{aligned}
|\langle u_j,\phi\rangle|
&=j^{-N}\left|\int_0^1\overline h_{j,N}(jx)\phi^{(N)}(x)\,dx\right|\\
&\leq j^{-m-1}\|g_j\|_{L^1}\|\phi^{(m+1)}\|_\infty
\leq\frac{M}{j}\|\phi^{(m+1)}\|_\infty\longrightarrow0.
\end{aligned}
$$

This is precisely [weak convergence of distributions](../../../../../weak-convergence-of-distributions.md), so $\boxed{u_j\to0\text{ in }\mathcal D'(0,1)}$. The extra [integration by parts](../../../../../integration-by-parts.md) beyond the growth exponent $m$ is what ensures decay.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the distribution theory course of the University of Oxford](../../../../split.md)
6. [Distribution theory course of the University of Oxford](../../../../../distribution-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
