<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Evaluate the supplied real [logarithmic derivative](../../../../../../logarithmic-derivative.md) at $2+it$. Since $1<2-\beta<2$, its positive summand is bounded above and below by constant multiples of $(1+|t-\gamma|^2)^{-1}$. On the other hand, differentiating the defining xi expression gives

$$
\frac{\xi'}{\xi}(s)=\frac1s+\frac1{s-1}-\frac12\log\pi
+\frac12\frac{\Gamma'}{\Gamma}(s/2)+\frac{\zeta'}{\zeta}(s).
$$

At real part two the last term is bounded by the [absolutely convergent](../../../../../../absolute-convergence.md) series $\sum\Lambda(n)n^{-2}$; the gamma [logarithmic derivative](../../../../../../logarithmic-derivative.md) is $O(\log t)$. Therefore

$$
\boxed{\sum_\rho\frac1{1+|t-\gamma|^2}=O(\log t).}
$$

For $\gamma\in[T,T+1]$, use $t=T$: each term in the displayed sum is at least $1/2$. Hence the number of zeros in that unit ordinate interval, counted with multiplicities, is $O(\log T)$. These are the [local zeta zero-count bound](../../../../../../local-zero-count-for-the-riemann-zeta-function.md) and the corresponding smoothed bound.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
