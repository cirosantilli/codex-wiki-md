<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [likelihood-ratio test](../../../../../likelihood-ratio-test.md) rejects for small $\lambda$. The [derivative](../../../../../derivative.md) of the [natural logarithm](../../../../../natural-logarithm.md) of its variable factor is

$$
\frac d{dt}\{n\log t+m\log(1-t)\}
=\frac{n-(n+m)t}{t(1-t)}.
$$

Thus $t^n(1-t)^m$ increases up to $n/(n+m)$ and decreases thereafter, tending to zero at both endpoints. Every nontrivial lower [level set](../../../../../level-set.md) of $\lambda$ therefore consists of two tails. For a prescribed [test size](../../../../../size-of-a-statistical-test.md) $0<\alpha<1$, the exact [critical region](../../../../../rejection-region.md) is

$$
\boxed{T<k_1\quad\text{or}\quad T>k_2},\qquad
0<k_1<\frac n{n+m}<k_2<1.
$$

Writing $F_{n,m}$ for the [cumulative distribution function](../../../../../cumulative-distribution-function.md) of the [beta distribution](../../../../../beta-distribution.md) with parameters $(n,m)$, the required two equations are

$$
\boxed{\begin{aligned}
k_1^n(1-k_1)^m&=k_2^n(1-k_2)^m,\\
F_{n,m}(k_1)+1-F_{n,m}(k_2)&=\alpha.
\end{aligned}}
$$

The first makes both cutoffs have the same [likelihood ratio](../../../../../likelihood-ratio.md); the second calibrates the [null hypothesis](../../../../../null-hypothesis.md) rejection [probability](../../../../../probability.md). Equivalently, the second left-hand side is

$$
\frac1{B(n,m)}\left\{\int_0^{k_1}t^{n-1}(1-t)^{m-1}\,dt+
\int_{k_2}^1t^{n-1}(1-t)^{m-1}\,dt\right\}.
$$

As the common [likelihood ratio](../../../../../likelihood-ratio.md) threshold increases from zero to one, this [probability](../../../../../probability.md) increases continuously and strictly from zero to one; hence the equations determine unique cutoffs. **The two tail probabilities need not each equal $\alpha/2$** when $n\ne m$. Exact calibration holds for every common rate because the given [null distribution](../../../../../null-distribution.md) of $T$ is independent of that rate. Boundary equalities have zero [probability](../../../../../probability.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
