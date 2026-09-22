<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [signed measure](../../../../../signed-measure.md) define its [total variation measure](../../../../../variation-measure.md) by

$$
|\mu|(E)=\sup\left\{\sum_{r=1}^m|\mu(E_r)|:E=\bigsqcup_{r=1}^m E_r,\ E_r\in\mathfrak M\right\}.
$$

The value at the empty set is zero. For disjoint [measurable sets](../../../../../measurable-set.md) $A_j$ with union $A$, any finite partition $E_r$ of $A$ gives

$$
\sum_r|\mu(E_r)|\leq\sum_j\sum_r|\mu(E_r\cap A_j)|\leq\sum_j|\mu|(A_j).
$$

Taking the [supremum](../../../../../supremum.md) proves one inequality. In the reverse direction choose, for the first $k$ sets, finite partitions approaching their variation values. Combining these partitions and the remaining set $A\setminus\bigcup_{j\leq k}A_j$ gives

$$
|\mu|(A)\geq\sum_{j=1}^k|\mu|(A_j)-\varepsilon.
$$

If one term is infinite, its partition sums can instead be made arbitrarily large. Letting $\varepsilon\downarrow0$ and $k\to\infty$ proves **[countable additivity](../../../../../countable-additivity.md)**, including infinite values. Thus $|\mu|$ is a [positive measure](../../../../../positive-measure.md). This uses only [countable additivity](../../../../../countable-additivity.md) of $\mu$, without assuming a [Hahn decomposition](../../../../../hahn-decomposition.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the real and harmonic analysis course of the University of Oxford](../../../../split.md)
6. [Real and harmonic analysis course of the University of Oxford](../../../../../real-and-harmonic-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
