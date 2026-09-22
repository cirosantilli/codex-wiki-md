<h1 id="3d/solution">Solution</h1>

↑ **Parent:** [3D](../3d.md)

For a nonempty [set](../../../../../set-split.md) $S\subseteq\mathbb R$, a [real number](../../../../../real-number.md) $s$ is its [supremum](../../../../../supremum.md) if every $x\in S$ satisfies $x\leq s$ and every [upper bound](../../../../../upper-bound-in-a-partially-ordered-set.md) $u$ of $S$ satisfies $s\leq u$. Equivalently, $s$ is an [upper bound](../../../../../upper-bound-in-a-partially-ordered-set.md) and, for every $\varepsilon>0$, some $x\in S$ has $s-\varepsilon<x\leq s$. The [least upper bound axiom](../../../../../least-upper-bound-property.md) states that every nonempty set of [real numbers](../../../../../real-number.md) bounded above has a real [supremum](../../../../../supremum.md).

Suppose $(a_n)$ is nondecreasing and bounded above. Apply the [least upper bound axiom](../../../../../least-upper-bound-property.md) to $S=\{a_n:n\geq1\}$, obtaining $s=\sup S$. For any $\varepsilon>0$, $s-\varepsilon$ cannot be an [upper bound](../../../../../upper-bound-in-a-partially-ordered-set.md), so there is $N$ with $a_N>s-\varepsilon$. For every $n\geq N$, monotonicity gives

$$
s-\varepsilon<a_N\leq a_n\leq s,
$$

so $|a_n-s|<\varepsilon$. This is precisely the definition of a [convergent sequence](../../../../../convergent-sequence.md). If $(a_n)$ is nonincreasing and bounded below, apply the proved case to $(-a_n)$; its limit is the negative of the [infimum](../../../../../infimum.md) of the original terms. Thus the [bounded monotone sequence theorem](../../../../../bounded-monotone-sequence-theorem.md) follows directly from the axiom:

$$
\boxed{a_n\to\sup_n a_n\ \text{in the nondecreasing case},\qquad
 a_n\to\inf_n a_n\ \text{in the nonincreasing case}.}
$$

## ↑ Ancestors (10)

1. [3D](../3d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
