<h1 id="b/5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For a [positive operator](../../../../../positive-operator.md), $\langle Tx,x\rangle\geq0$. We show directly that every nonreal or negative real $\lambda$ lies in the [resolvent set](../../../../../resolvent-set-of-an-operator.md).

If $\operatorname{Im}\lambda\ne0$, the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) and reality of $\langle Tx,x\rangle$ give

$$
\|(T-\lambda I)x\|\|x\|\geq|\langle(T-\lambda I)x,x\rangle|\geq|\operatorname{Im}\lambda|\|x\|^2.
$$

Thus $T-\lambda I$ is bounded below, hence injective with closed range: a convergent sequence of outputs has Cauchy preimages, whose limit maps to that output. Its adjoint is $T-\bar\lambda I$, which has trivial [kernel](../../../../../kernel-of-a-linear-map-split.md) by the same estimate. The identity $\operatorname{Ran}(A)^\perp=\ker A^*$, proved by the same inner-product calculation as in (i), makes its range dense. Being closed and dense, it is all of $X$, and the lower bound makes the inverse bounded.

If $\lambda<0$ is real, positivity gives $\langle(T-\lambda I)x,x\rangle\geq(-\lambda)\|x\|^2$, so the same argument applies with lower bound $-\lambda$. Here the operator is [self-adjoint](../../../../../self-adjoint-operator.md), so its range is dense because its own [kernel](../../../../../kernel-of-a-linear-map-split.md) is zero. Hence

$$
\boxed{\sigma(T)\subseteq[0,\infty).}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [B](../../../b.md)
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
