<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $Z=\overline{\operatorname{span}}\{x_n:n\geq1\}$. If $Z\ne X$, part (a) provides a nonzero bounded functional annihilating $Z$; normalize it to have [norm](../../../../norm.md) one. Density of the sequence in the dual unit ball gives an index $n$ with $\|f_n-f\|<1/4$. Since $f(x_n)=0$ and $\|x_n\|\leq1$,

$$
|f_n(x_n)|\leq\|f_n-f\|<\frac14.
$$

But the hypothesis and reverse [triangle inequality](../../../../triangle-inequality.md) give

$$
|f_n(x_n)|\geq\frac12\|f_n\|>\frac12\left(1-\frac14\right)=\frac38,
$$

a contradiction. Therefore **the span is dense**.

If $X'$ is [separable](../../../../separable-topological-space.md), its unit ball has a countable [dense set](../../../../dense-set.md). For each nonzero $f_n$, the definition of its [norm](../../../../norm.md) permits choosing $x_n$ in the unit ball with $|f_n(x_n)|\geq\|f_n\|/2$; choose zero for a zero functional. The preceding result gives a dense countable span over $\mathbb Q$, or over $\mathbb Q+i\mathbb Q$ in the complex case. Thus **$X$ is [separable](../../../../separable-topological-space.md)**.

The converse fails: $\ell^1$ is [separable](../../../../separable-topological-space.md), since finite rational-coordinate sequences are dense, but $(\ell^1)'\cong\ell^\infty$ is not [separable](../../../../separable-topological-space.md). The dual identification sends a bounded sequence $a$ to $x\mapsto\sum_na_nx_n$, isometrically; conversely a bounded functional is determined by its values on the [coordinate vectors](../../../../coordinate-vector.md) and hence has this form by truncation. The uncountable family of zero-one sequences in $\ell^\infty$ has pairwise [distance](../../../../distance.md) one, which no countable [dense set](../../../../dense-set.md) can approximate within a radius smaller than $1/2$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the analysis course of the University of Oxford](../../../split.md)
5. [Analysis course of the University of Oxford](../../../../analysis-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
