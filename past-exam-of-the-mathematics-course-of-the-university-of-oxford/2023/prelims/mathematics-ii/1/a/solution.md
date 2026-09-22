<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a nonempty [set](../../../../../../set-split.md) $A\subseteq\mathbb R$, a [supremum](../../../../../../supremum.md) is a [real number](../../../../../../real-number.md) $s$ such that $a\leq s$ for every $a\in A$, and every [upper bound](../../../../../../upper-bound-in-a-partially-ordered-set.md) $u$ of $A$ satisfies $s\leq u$. Equivalently, $s$ is an [upper bound](../../../../../../upper-bound-in-a-partially-ordered-set.md) and, for every $\varepsilon>0$, some $a\in A$ satisfies $a>s-\varepsilon$. By [completeness of the real numbers](../../../../../../completeness-of-the-real-numbers.md), it exists whenever $A$ is nonempty and bounded above.

An increasing [monotone sequence](../../../../../../monotone-sequence.md) satisfies $a_{n+1}\geq a_n$ for every $n$; a [bounded sequence](../../../../../../bounded-sequence.md) satisfies $|a_n|\leq M$ for some finite $M$ and every $n$. Put $s=\sup\{a_n:n\geq1\}$. Given $\varepsilon>0$, the defining property of the [supremum](../../../../../../supremum.md) supplies $N$ with $a_N>s-\varepsilon$. For every $n\geq N$, [monotonicity](../../../../../../monotonic-function.md) gives

$$
s-\varepsilon<a_N\leq a_n\leq s.
$$

This is exactly the definition of [convergent sequence](../../../../../../convergent-sequence.md), so the [bounded monotone sequence theorem](../../../../../../bounded-monotone-sequence-theorem.md) gives $\boxed{a_n\to s}$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
