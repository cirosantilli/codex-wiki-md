<h1 id="a/1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We use [successive approximation for quotient operators](../../../../../successive-approximation-for-quotient-operators.md). Fix $y$ with $\|y\|<1$. The hypothesis gives $x_0$ with $\|x_0\|<1$ and $\|y-Tx_0\|<\delta$. Inductively, if

$$
r_n=y-T\sum_{k=0}^{n-1}x_k,\qquad\|r_n\|<\delta^n,
$$

apply the hypothesis to $r_n/\delta^n$, obtaining $x_n$ with $\|x_n\|<\delta^n$ and $\|r_n-Tx_n\|<\delta^{n+1}$. If a residual is zero, take all remaining terms zero.

The [series](../../../../../series-mathematics.md) $\sum x_n$ converges in the [Banach space](../../../../../banach-space-split.md) $X$ because $\sum\|x_n\|<\sum\delta^n=(1-\delta)^{-1}$. Write its sum as $x$. The [continuity](../../../../../continuous-function.md) of $T$ and the residual estimate give

$$
Tx=y,\qquad\|x\|<(1-\delta)^{-1}.
$$

Scaling now yields

$$
\boxed{B_Y(0,1-\delta)\subseteq T(B_X(0,1)).}
$$

This ball inclusion proves that **$T$ is a [quotient operator](../../../../../quotient-operator.md)**. Completeness of $Y$ was unnecessary: the convergent [series](../../../../../series-mathematics.md) is constructed in $X$ and its [image](../../../../../image-of-a-function.md) has limit $y$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../split.md)
6. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
