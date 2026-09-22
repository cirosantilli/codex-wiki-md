<h1 id="6/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

By the [mean value theorem](../../../../../../../mean-value-theorem.md), $|f(x)-f(y)|\leq A|x-y|$ for all real $x,y$. Thus $f$ is a [contraction mapping](../../../../../../../contraction-mapping.md) on the [complete metric space](../../../../../../../complete-metric-space.md) $\mathbb R$. Starting from arbitrary $x_1$, define $x_{n+1}=f(x_n)$. Induction gives $|x_{n+1}-x_n|\leq A^{n-1}|x_2-x_1|$. For $m>n$, the [triangle inequality](../../../../../../../triangle-inequality.md) and a [geometric series](../../../../../../../geometric-series.md) yield

$$
|x_m-x_n|\leq\frac{A^{n-1}}{1-A}|x_2-x_1|\longrightarrow0.
$$

Hence $(x_n)$ is a [Cauchy sequence](../../../../../../../cauchy-sequence.md) and [completeness of the real numbers](../../../../../../../completeness-of-the-real-numbers.md) supplies a [limit](../../../../../../../limit-of-a-function.md) $x$. The [Lipschitz continuity](../../../../../../../lipschitz-continuity.md) of $f$ implies $f(x)=\lim f(x_n)=\lim x_{n+1}=x$. Thus the limit is a [fixed point](../../../../../../../fixed-point.md), independently of the initial value. If $y$ were another, $|x-y|\leq A|x-y|$ would force $x=y$. This proves the [contraction mapping theorem](../../../../../../../contraction-mapping-theorem.md) in this setting, with error estimate

$$
\boxed{|x-x_n|\leq\frac{A^{n-1}}{1-A}|x_2-x_1|.}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
