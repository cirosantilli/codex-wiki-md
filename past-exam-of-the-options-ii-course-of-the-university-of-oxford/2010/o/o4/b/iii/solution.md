<h1 id="o/o4/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Under the null, replace both parameters by a common $r$. The likelihood becomes

$$
L_0(r)=\binom{2N}n\binom{2M}m
r^{n+m}(1-r)^{2(N+M)-n-m}.
$$

The pooled maximum-likelihood estimate is

$$
\boxed{\widehat r=\frac{n+m}{2(N+M)}.}
$$

Under an interior null $p=q=r$, part (ii) gives a centered asymptotic normal difference with [variance](../../../../../../variance-split.md) $r(1-r)(1/(2M)+1/(2N))$. The [law of large numbers](../../../../../../law-of-large-numbers.md) makes $\widehat r\to r$ in probability. By Slutsky's theorem, replacing $r$ by this consistent estimate gives

$$
\boxed{Z=\frac{\widehat p-\widehat q}
{\sqrt{(1/(2M)+1/(2N))\widehat r(1-\widehat r)}}\xrightarrow dN(0,1).}
$$

For the two-sided alternative, reject when $|Z|>z_{1-\alpha/2}$, the corresponding standard-normal [quantile](../../../../../../quantile-function.md). This has asymptotic [significance level](../../../../../../significance-level.md) $\alpha$.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [O4](../../../o4.md)
4. [O](../../../../o.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the options II course of the University of Oxford](../../../../../split.md)
7. [Options II course of the University of Oxford](../../../../../../options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
