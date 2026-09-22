<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write a [Blaschke product](../../../../../blaschke-product.md) as $B(z)=\lambda z^m\prod_n b_{a_n}(z)$, where $a_n\ne0$, $|\lambda|=1$, and the zeros are counted with [multiplicity](../../../../../multiplicity-mathematics.md). With normalized angular measure $dm=d\theta/(2\pi)$, [Jensen's formula](../../../../../jensen-s-formula.md) for each [Blaschke factor](../../../../../blaschke-factor.md) gives

$$
\int\log|b_a(re^{i\theta})|\,dm=\log\max(r,|a|).
$$

Indeed, the mean of $\log|a-re^{i\theta}|$ is $\log\max(r,|a|)$, while $\log|1-\overline a re^{i\theta}|$ has mean zero by the [mean value property for harmonic functions](../../../../../mean-value-property-for-harmonic-functions.md). Each factor has modulus at most one. Applying the [monotone convergence theorem](../../../../../monotone-convergence-theorem.md) to the negative logarithms of the finite products yields the [radial logarithmic mean of a Blaschke product](../../../../../radial-logarithmic-mean-of-a-blaschke-product.md):

$$
\int\log|B(re^{i\theta})|\,dm=m\log r+\sum_n\log\max(r,|a_n|).
$$

The [Blaschke condition](../../../../../blaschke-condition.md) implies $\sum_n-\log|a_n|<\infty$: only finitely many zeros have modulus below $1/2$, and $-\log t\le2(1-t)$ for $1/2\le t<1$. Every summand tends to zero and is bounded in absolute value by $-\log|a_n|$. The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) for this series, together with $m\log r\to0$, therefore gives

$$
\boxed{\lim_{r\uparrow1}\int\log|B(re^{i\theta})|\,dm=0.}
$$

This also covers finite products and constant unimodular products. Zeros on a circle create integrable logarithmic singularities and do not change the conclusion.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

## ← Incoming links (1)

- [Solution](c/solution.md)
