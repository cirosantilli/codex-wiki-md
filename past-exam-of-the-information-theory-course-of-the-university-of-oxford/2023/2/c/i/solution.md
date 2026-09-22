<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For every $x^n\in A^{n,\varepsilon}$, the defining [typical set](../../../../../typical-set.md) constraint implies

$$
2^{-n(H(p)+\varepsilon)}\leq p_n(x^n)\leq2^{-n(H(p)-\varepsilon)}.
$$

Let $S_n=A^{n,\varepsilon}\cap B^{n,\varepsilon}$. Summing the lower [probability mass](../../../../../probability-mass.md) bound over $S_n$ gives

$$
1\geq\Pr(X^n\in S_n)
=\sum_{x^n\in S_n}p_n(x^n)
\geq |S_n|2^{-n(H(p)+\varepsilon)}.
$$

Therefore

$$
\boxed{|A^{n,\varepsilon}\cap B^{n,\varepsilon}|\leq2^{n(H(p)+\varepsilon)}.}
$$

The [sample mean](../../../../../sample-mean.md) constraint can only shrink the [typical set](../../../../../typical-set.md), so this [cardinality](../../../../../cardinality.md) upper bound holds for every positive integer $n$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the information theory course of the University of Oxford](../../../../split.md)
6. [Information theory course of the University of Oxford](../../../../../information-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
