<h1 id="27j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $R_t=0$ when no record has occurred below $t$, the needed convention for the maximum of an empty set. Assume $F(t)<1$ and write $S(t)=1-F(t)$. Given the latest record $v_k<t$, the chance that the next one exceeds $t$ is $S(t)/S(v_k)$. Multiplying this by the joint density from part (a) leaves

$$
S(t)\prod_{j=1}^k\frac{f(v_j)}{S(v_j)}
$$

on the ordered simplex $0<v_1<\cdots<v_k<t$. Its [integral](../../../../../../integral.md) is $S(t)\Lambda(t)^k/k!$, where $\Lambda(t)=\int_0^t f(s)/S(s)\,ds=-\log S(t)$. The $k=0$ probability is directly $S(t)=e^{-\Lambda(t)}$. Hence

$$
\boxed{R_t\sim\operatorname{Poisson}(\Lambda(t)),\qquad\lambda(t)=\frac{f(t)}{1-F(t)}.}
$$

This is [Poisson record counts in cumulative hazard coordinates](../../../../../../poisson-record-counts-in-cumulative-hazard-coordinates.md); the instantaneous rate is the original distribution's [hazard function](../../../../../../hazard-function.md). If the distribution has a finite upper endpoint and $t$ reaches it, $F(t)=1$ and infinitely many record values lie below $t$ almost surely; there is then no finite-parameter Poisson law. The finite-hazard assumption is thus necessary for the literal assertion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [27J](../../27j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
