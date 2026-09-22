<h1 id="a/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $|\lambda|>\|T\|$, write $T-\lambda I=-\lambda(I-T/\lambda)$. The [Neumann series](../../../../../neumann-series.md) applies to $T/\lambda$, so $\lambda$ is outside the [spectrum of a bounded operator](../../../../../spectrum-of-a-bounded-operator.md). Thus $\sigma(T)\subseteq\{\lambda:|\lambda|\leq\|T\|\}$ and $r(T)\leq\|T\|$.

The polynomial [spectral mapping theorem](../../../../../spectral-mapping-theorem.md) gives $\sigma(T^m)=\{\lambda^m:\lambda\in\sigma(T)\}$, and hence

$$
r(T)^m=r(T^m)\leq\|T^m\|.
$$

Taking $m$th roots and then the limit, whose existence is allowed, proves

$$
\boxed{r(T)\leq\lim_{m\to\infty}\|T^m\|^{1/m}.}
$$

Only this inequality is required; the reverse inequality is the additional content of the full [spectral radius formula](../../../../../spectral-radius-formula.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the analysis course of the University of Oxford](../../../../split.md)
6. [Analysis course of the University of Oxford](../../../../../analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
