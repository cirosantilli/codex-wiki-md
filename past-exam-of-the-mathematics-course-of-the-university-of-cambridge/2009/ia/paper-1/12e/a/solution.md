<h1 id="12e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Riemann integrable](../../../../../../riemann-integrable-function.md) function on a closed interval is bounded and has equal [upper and lower Darboux integrals](../../../../../../upper-and-lower-darboux-integrals.md). More explicitly, for a [partition of an interval](../../../../../../partition-of-an-interval.md) $P:a=x_0<x_1<\cdots<x_m=b$, define the [Darboux sums](../../../../../../darboux-sum.md)

$$
L(f,P)=\sum_{j=1}^m\inf_{[x_{j-1},x_j]}f\,(x_j-x_{j-1}),\qquad U(f,P)=\sum_{j=1}^m\sup_{[x_{j-1},x_j]}f\,(x_j-x_{j-1}).
$$

Then **[Riemann integrability](../../../../../../riemann-integrable-function.md) means**

$$
\boxed{\sup_P L(f,P)=\inf_P U(f,P),}
$$

and this common value is the [Riemann integral](../../../../../../riemann-integral.md). Equivalently, the [Riemann integrability criterion](../../../../../../riemann-integrability-criterion.md) requires that for every $\varepsilon>0$ some [partition of an interval](../../../../../../partition-of-an-interval.md) satisfies $U(f,P)-L(f,P)<\varepsilon$. Indeed, the common [partition refinement](../../../../../../partition-refinement.md) of two partitions increases each lower [Darboux sum](../../../../../../darboux-sum.md) and decreases each upper [Darboux sum](../../../../../../darboux-sum.md), so equality of the two extremal values is equivalent to arbitrarily small gaps.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12E](../../12e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
