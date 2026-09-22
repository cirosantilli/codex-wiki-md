<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Neumann series](../../../../../neumann-series.md) criterion states that $\|A\|<1$ for a [bounded linear operator](../../../../../continuous-linear-operator.md) on a [Banach space](../../../../../banach-space-split.md) implies

$$
(I-A)^{-1}=\sum_{n=0}^{\infty}A^n,
$$

with convergence in the [operator norm](../../../../../operator-norm.md). In particular, $\|T\|<1$ suffices for invertibility of $I-T$.

If $|\lambda|>\|T\|$, apply this criterion to $A=T/\lambda$. It gives

$$
(\lambda I-T)^{-1}=\lambda^{-1}\sum_{n=0}^{\infty}(T/\lambda)^n.
$$

Thus no such $\lambda$ belongs to the [spectrum](../../../../../spectrum-functional-analysis.md), and

$$
\boxed{r(T)\leq\|T\|.}
$$

For each integer $j\geq1$, if $|\lambda|^j>\|T^j\|$, then $\lambda^jI-T^j$ is invertible by the same argument. The commuting factorization

$$
\lambda^jI-T^j=(\lambda I-T)\sum_{k=0}^{j-1}\lambda^{j-1-k}T^k
$$

then gives a bounded two-sided inverse for $\lambda I-T$, namely the displayed sum multiplied by $(\lambda^jI-T^j)^{-1}$. Hence every $\lambda\in\sigma(T)$ satisfies $|\lambda|^j\leq\|T^j\|$. Taking the [supremum](../../../../../supremum.md) over the [spectrum](../../../../../spectrum-functional-analysis.md) and then the [infimum](../../../../../infimum.md) over $j$ proves

$$
\boxed{r(T)\leq\inf_{j\geq1}\|T^j\|^{1/j}.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analysis I course of the University of Oxford](../../../../split.md)
6. [Functional analysis I course of the University of Oxford](../../../../../functional-analysis-i-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
