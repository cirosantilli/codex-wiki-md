<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The relation between $B$ and $W$ is the linear equation $dB_s=dW_s-\beta B_sds$ with $B_0=0$. Multiplication by the deterministic integrating factor $e^{\beta s}$ and the [Itô product rule](../../../../../ito-product-rule.md) give

$$
d(e^{\beta s}B_s)=e^{\beta s}\,dW_s.
$$

Hence

$$
\boxed{B_s=\int_0^se^{-\beta(s-u)}\,dW_u
=W_s-\beta\int_0^se^{-\beta(s-u)}W_u\,du.}
$$

The second equality follows by [semimartingale integration by parts](../../../../../semimartingale-integration-by-parts.md). It expresses $B$ as an explicit function of the continuous path of $W$, using only an ordinary time integral. This inversion holds before changing measure; $W$ is already a [continuous semimartingale](../../../../../continuous-semimartingale.md) under the original measure.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the stochastic differential equations course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations course of the University of Oxford](../../../../../stochastic-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
