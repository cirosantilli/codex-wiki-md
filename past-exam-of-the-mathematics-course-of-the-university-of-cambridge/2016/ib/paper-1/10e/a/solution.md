<h1 id="10e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

We prove [prime avoidance](../../../../../../prime-avoidance.md) by contradiction. Remove any [prime ideal](../../../../../../prime-ideal.md) contained in another one on the list; this leaves the same union. If the [ideal](../../../../../../ideal.md) $I$ is contained in none of the remaining [prime ideals](../../../../../../prime-ideal.md), choose $a_i\in I\setminus P_i$. For every $j\ne i$, incomparability lets us choose $b_{ij}\in P_j\setminus P_i$. Set

$$
b_i=\prod_{j\ne i}b_{ij},\qquad c=\sum_i a_i b_i.
$$

For a one-element list, use the empty product $b_1=1$. By the defining property of a [prime ideal](../../../../../../prime-ideal.md), $b_i\notin P_i$, and also $a_i b_i\notin P_i$. But $b_j\in P_i$ for every $j\ne i$. Thus all summands except $a_i b_i$ lie in $P_i$, and consequently $c\notin P_i$ for every $i$. On the other hand, $c\in I$ because each $a_i\in I$. This contradicts the assumed containment in the union. Therefore

$$
\boxed{I\subseteq P_i\text{ for at least one }i.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10E](../../10e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
